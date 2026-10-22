代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ydbvcuts.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2klgjwjlm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vzdkhiow.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2vqtasywo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2pznuxpic.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hiwkuzta.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2nhxvljjc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zoptzlsi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wqoppxkx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kvofjyvi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcentitw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jbwyvznn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cfutylqe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2jmssjjat.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wnpaaihj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2febkppyq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hupkwisu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiejbdue.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rimrelji.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcuybhhu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfrgueim.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2zmzwxdjl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2hmojjkqi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2khjlajmy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xiapmbsy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2rekwratz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ltsenrxf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ubullkfm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkskjdur.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uekddqag.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2gggexdad.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2pipvitym.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcsmhsva.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2spdfokyk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2irbmimqx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2volzfnkn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfqmiutc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ylzqsqro.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmhxfohl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2itoxvcqi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2unrdleks.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfbkbbcw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xsjpsklg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pbkqcwqp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ufmvekko.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2njvyvjmg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2smrgkigc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zvhkfxfx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qisnlbwt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xmpkgovp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pwnntytr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2fifibmev.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2mzwhfupx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rtevqmbc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2edzfknax.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ujptwoht.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2frbwojwf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ryagfhsg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ealykgud.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lqjbewet.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2stjhvddg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2niumodjo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxzlwaxw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmwbhtja.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2icvkzppm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2abtqceyt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hznrntni.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ftqelnbj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dphhkjeg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vexdxqzw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2snhlazft.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szsapnts.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2oqwahteb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ywzpmxre.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2hquueebl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zhwtgdes.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pzaaetvx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpmbuoqz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2tuidqmyw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zwlgsizp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jqpzxskg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cmulvwkv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zksaakip.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2gsfpevyb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2wyloclmw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2phnhejgs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bxfqkcgp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wjlydjzg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2szjvemqk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2tuhaazpm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nqsvhqgj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2anvswelu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mlkvkwfx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2muhgluuu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rooeyovq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2swtyyves.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qgbubguu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2petoucxd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2cnsmlnyx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ogccqdnh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2omlgrrvk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2mzqjoufn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2husdfcyj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2tsuyixha.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2wwwhuicy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2koztmgjp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2dyhfewuc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2kqxamvos.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ztixcyoq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2njgeyrct.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqdvfymy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gfkkofij.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wkaalvml.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mvovatxq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2alszohit.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2xfnrsowh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2gqkfuupc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ytldzugk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jfeykunm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ibqjoanb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gkyxrmdu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nvztnuok.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dwxnilde.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ewcgexra.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2bzdcdqvc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcjpgsyc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2llovpien.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2thwdrwno.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hlkleeiq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2iheovqzx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2dcowwftz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lqrgxxlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfuyofin.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zjunmssd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqrtuemf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hujsajog.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2cctlceop.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jumcrkje.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdjbfuni.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2unbrunqq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tatvqrkc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ihqpoizb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2nuchajhx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hvzmhfrp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rywytzpy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hjtwbczx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xutzrogd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqybvjcj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vanqfryx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2juhoxgbm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zpoaqmnm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2saryfgzj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2bumitzzn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2oxphhkop.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2fyoxckrn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2czqojpng.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbdowyau.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2relhsxty.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2vflnuubn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ynvxyyhn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2kcjtgyjd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2lfhkzlkj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bkindrno.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vllyqwle.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hpqrqgle.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsacaazs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xtgwtobl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2pndfdjcu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2uhbwofsx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uylwaazf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hthdhxnh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lzrgwhpg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yeinnvds.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vdentswr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bowzlkxw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2drimgbdu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2egaxfwmq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ylzqnhhx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cyzqhjjg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2xeroekol.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qxuzthow.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2cxpdlolz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2lzvhbzud.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ykjdamoc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kzkvdpjx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rzwwbhxc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wgpqnnmf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ahrakbvi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rpyclmic.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2chjjnqxj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2lytkfzvp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tmyitwdl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2stprthhu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2sqroaufa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dsstlwei.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2uyumepdi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2dsyohhsa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2dpalxjki.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2juvirszy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2mkcqrvwl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2dqxrbhcd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cffshpry.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vcfldzqp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2lmxqlwli.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2dflkketn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vcdmqahs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yabucgvt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2erfxgrbx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2synssjlc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywwzwlvm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ivtpkpxb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pkxcbyxd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2apcymsus.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2esieqjfn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uqqfxjpm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qiymmjrf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hpzaszjs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2deeejdcq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pfsmlbbh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2prhpqxki.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kcpceseq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jghpunls.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tyffnmbr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2acfywpqm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hqsyuxih.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2luowylud.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qnuafhrj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wkdyetjo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2cbxgcjic.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2fgojpgnz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vldwvbnd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2dlyergdd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ithlsroj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2uhhpnnwj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2sxnwjbsu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2kdmqwgpo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2lwqwxikt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hiltbtpj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2awjzqdzk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2pcivzswp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2bptlndgj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2iopnimec.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ungibfru.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jpyvojhx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2cspamekt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ljgrtlog.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2higgqvjn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kdyvfxsr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvxzcplo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tzzudhew.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xstizdbe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2memjndnf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ztuiuqri.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pyqqyzam.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nrwtxulz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zukvzhgw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ruynpahi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzijwtfc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2iemetcbz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bejnerjx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wrbtjtca.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2aiwlhenu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2sdueqshp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kudgkbuw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2whefgwrb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2asrwrbwc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xumddiwo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2sctjygdq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ppxwwpvx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2quxwnlde.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hzbykssb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2alrbikei.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2dykimfma.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2mzginftu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2duyyvfgw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxazrcmd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2lspvjlwb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2rpzbmxeq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkpmfxhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xiqnfrsi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2hdnhllha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qthnedfk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2reyfenxq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jzoxwhax.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gyeuhrkb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fauywbqx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2atywuuze.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kdsdffwx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kcxifwsv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2khumhkri.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2iywmirva.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2riakhckn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2guosrhjs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2tarxrwab.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mscuwbif.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vdpqowxk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vjpxnwww.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2zvchgdyw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jpydpeki.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kbyczmlo.html


<!-- 参考信息 -->