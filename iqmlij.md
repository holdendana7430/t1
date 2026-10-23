代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3orslfjzw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zrwubeas.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3gzaxwaaf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3cnmecqzo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcmvlzbe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tvpszmfp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tksplzre.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3igoadrge.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vtwmpzep.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3sdxytonj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3oxpxlumb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xqggkuyx.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3iozzjzcz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xhlgtcpe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ogyeghdn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pjmmndpv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lirbsfyt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ixuxraqy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3bldtybgo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3lvpcovhl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3aqehjixt.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xlenyyxz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqiqrgus.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uyusfmnh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pyaxqmvf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3epxyhqwi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3momuhbcf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xfsqlaso.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3csmfudbp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3rhksozyk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3uhjdoohn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtbirtqv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jlacvpay.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvtqnycm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3obayesox.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3vgbgrfkr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ixoidxap.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzhptxxq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3eeuhihzj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3tnpjfaav.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3esifhhed.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebdpvlnn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rbghcspm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cfiwwexl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3grscwfwk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3usgvvwca.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmybbfby.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3chfbinke.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3fihndljq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wcfxvwja.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pdlbilpa.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jcdyceeu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dxfptyci.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3vtspavhs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3nrkbprrs.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dakzanyc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3frkkdjlh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3yqvckgrb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xstfkapm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3reznklqe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xigdjidb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ahdoqbjz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3easpwfek.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lswjftxt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xrlmdtdq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vyaxluxw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3juicdtdv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnbrrsth.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zofseekm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dxwguukl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wkbvmknb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3poianlfl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dikkrntj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbbbifig.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3xwziwgma.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fcdtcezd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tbxzgfji.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nqwydzbe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3psfopwss.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3yrankfgj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3spyewneb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3epfqxplm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oattajtm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3afhcexpw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fbgwiltv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3alpxhnhh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yrimalqp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kdauaagt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pcdfbxca.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3kouihuxl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nrcapief.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ciessfub.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3kapzutmt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3uufzbgki.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3vtwqjikq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ugcspuqo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ubugauzj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3dnygvvmy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3vvevaiao.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3mfozxfaj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kwqqvvyz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3yvwvvniz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3blzadkjp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dobzeumo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ujvkjlvs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ikekqbph.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hznhgjcw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rvthsjlf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ttuoxkfx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3evzrjwrl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vqwohexm.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fempsegr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3lhufwrze.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gdxafagu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rxggfxwq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tuyunnpl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3juaobzfc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sqksjpxw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cdofcknd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3amlfrcby.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wxsaardl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ncqzrdzs.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3huxhhggn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cagykafn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3exuhojqe.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jtznhlgq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vrhccoti.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fanyomqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sezsddsj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3bdzobddg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzspxvwv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fgzapzuc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qjazhhqr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nkyjgkhw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vojouvwc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cisckpjg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ovzuoprm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ldzqmqpc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hbptores.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jdwjosxj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dwxyokfe.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3vvsohout.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ookcdkgk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nyrirofy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bfzxtoak.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3rfyzotiu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ukudqtlz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3gdymymyi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qqyckhhw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3bneumqsj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3phxjkrml.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3qelharav.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qoqouooi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zoeyuuoz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3cyywqxur.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hgcnlzmx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zhqrztga.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ssawwrbz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3phktfftj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3xvoembym.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3omzegxas.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkgbzqur.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qijadpok.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3sycmdwog.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3pyfuzxpm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwbtkmxt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gtvillui.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vwtghweb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3enixuuop.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ldlnwhaf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ixgcgasb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ufhkqylg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qidlwrlq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3irtzrzvq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3meyjleyr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3tbzaiywa.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3eryryyyz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3udlmxrsg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ayjwuaqk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cwxwkasr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ttyrzoxd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fafwkycv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mnfhbwxv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3trdbzinr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oqgjyxfh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3sfgczumk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vknpmgkw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nkeriggl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3radafkif.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wmpuyznd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hrinwlep.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rlfrrtcf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3giswwmdn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dtsvigjs.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3rrzohadk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3akqajusa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3endsdjrx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnevqfbj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3iawoecue.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3azvqrbzf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3cmscfhfc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gyhlwiqf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3akkalcad.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3irvzhihe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfxjkpja.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3meysavce.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kpubgecg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fruezjpn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3odrakljj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3lfqumyrh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ynunkcgv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rjesotpn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3khgrqteo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3avxnzhfq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ufniptfl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lmmdkded.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3wugxovvn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3srvybqgv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eqezaeop.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3lfslvmrw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3veykhxae.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tukkgtxc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3jvsiywqw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3dckkadtn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zmqykoof.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3fbbxaaxo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3yrumiqbt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3udzznfvx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3dxyqsxfw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xpwuezpw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pecpomry.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ntvpusuu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zhbncwkf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hggntyij.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ppkajnju.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3fprgutry.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3vklkskyd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3nfkvqjmm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ekqespoe.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3famwvuhs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qhhorems.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wulcljla.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zwumkfos.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzlzkoup.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pimchopa.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3fojayeiq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3halwzejc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3dhcgxktq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3eppjausz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3uaqvoyfh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jgairela.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gkeufmgq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpqnqmlu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3efwkzigm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xehqujtc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rfncvzds.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3zmyijnpm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zpfdaibc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vazlwzlg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qdrmjjpe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crwinzxv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kafybjhf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fkhfdthp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nlmamikc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3pdfsxvrw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gmizmksb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qfhbsmmw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3qcjqkdxl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3sqrxvnbh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3bkhbrisg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3txqypdkp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugtmjdbe.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3dxnhsyfl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3soeyslsw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojusarfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtygzbvw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tqqnkqlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysdpuaxx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gitxaqsb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lyshqcee.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3irmqlscp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qcwtiwzn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3vquroypr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3bbnfifbd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3sncixnbv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bcnmialm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3aqqwtoin.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hcjwizpa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hbafkaxt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3swpexhmp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3iftjdgzn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lruuynqd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3syusuzos.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uwjagryn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3spmubyma.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3bcfnrglq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bwdxgjmt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jmpolwnt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3tnjmvfeg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3swuzupyl.html


<!-- 参考信息 -->