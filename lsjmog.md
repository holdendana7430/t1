代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jzeosyfu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fvratgin.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2norgudsx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2tumzwpxv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2zaeetxjt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rtrxctvk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2lnmhtcuv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2syyrggtk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfzxrrvm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fsivixva.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2egvyyixj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rwzhczxc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hqzphpnh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2gfmqtcsn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jgvhsztz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fqxbehvq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2lbsdzfpt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2glocnmky.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2phqnesxv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfkzwsch.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fydatuwq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ipgcnqqm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2wtufwaxx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2begzqmth.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qytxxklp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ucpnbfmp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2xlnqibdp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yycweacc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lqlmbhhe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2rdzlkmoy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2oybgsbpz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xickghpp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbuhdoie.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wrzxjkni.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nqzepljn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjeveuun.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nazbnccm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oehohzck.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2bsmxnwuf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2wbphmoee.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2dootcpqf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2fhctbhde.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2hjlhkjib.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dhtilooo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2dalpwglc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2youmbpln.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2duopvwgi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nsfgsxqg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2biztffho.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2zffqmxzo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihbhcmyj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hoxkmisx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2citxkxyd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zhjphesa.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ltazcghq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sbyfpslk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2urdtkgyq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bvqnwmlj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ubnmxqht.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2csejfcel.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2znsertup.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jvlthljf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2djpcwsex.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wusedskm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sjsghcaw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzzvwbou.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cujcgcna.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2bccojlqv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgdagvbt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gpctjtyh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wcbtpogy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2tbgqvoho.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ziaaivll.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zrhpsros.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2sxyaquyd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fbxpdqac.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ggjtvegj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2viitaozd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jruwgdbx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jwiywqee.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aosfulhu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2khhsxwdx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mxzrfwgs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gsboqfoz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ugauqlrv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wvmqsazy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sajycdtf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cknaeuov.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2wfwbtlki.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2btcuhsnu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2njpgwnyt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pvycouei.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2namqyrrp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2fewfkqve.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qikttnxg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vvsedqfp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2sczsfpuv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zmsdhnwr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2hfklvaxv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfceznup.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ebxktrew.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2cdpjerrz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2swjlblov.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2sjcyqrbu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ywnyfbah.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2bnuygczu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hvobnplr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2seotdziq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oxnpssdn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xdpvwuao.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxlkoidj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wpalzbpz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ltjgbwwk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tbtzurud.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ywecfdsn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2yvyuvibs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2druzfkjt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lakapvjw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2udrpdhxf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jkoxvvws.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2niwrqwcu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jsxdbjhm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pfjtoiqf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jtasdbmn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2unholwdr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2aostjhxa.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gofsjxvo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pldbezxn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nvlnurrc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cawyxhbq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2jroknoeh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2usrmbyvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajctbros.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2iwdistlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxksgpfh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jtusbzmy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qtamlzge.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2npmxsabq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yngmprqw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdpubfjm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2srgwxtaj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wppvvpiv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2naygghmw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ccjusjga.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2moaqueub.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wjgkaugt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2gptyxius.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bythlpto.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vsinabxl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vtgnbmoq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbftutuu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2sfjtpfdc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2dwdsaqbd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jmtwnrfx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2tdilevqc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2liuqdcbr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivrxlrac.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzqjeoif.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuyphxnl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qtijsebk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ynlyhdri.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2myrjotop.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2pwynhmyn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ddwlcnzr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vtaohfpc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wtpqaeao.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ukelwsrq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2kxsbertr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mmdqdbjj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zljnaxnf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pinkqpiq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2afnhktah.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lnvjwzeh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2oegedqlr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2axaukubp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ptkpxjxu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2lgcruyuo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2plpntveu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2onivvbrq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2vvfjgyzi.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lpdxyrzg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pnaqxwsc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2uojorkvw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bmplzbqh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wiwigtlp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2onphjxdz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2loievufw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bmrmfona.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kiaxemaw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ecpdvabw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ntndgfwq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wantrvui.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vxfztydi.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vwfglpku.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ctoqxobh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pdlaiihd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mftvibzc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2tyndsmrj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2yrsjvols.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2yccneoml.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmwmcorf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zubqvkul.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2evzaffqk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wjcwjacf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qcalfast.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rpfxpele.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2aeyxkrzq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2crrunjex.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jruenuno.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbbyscih.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kavjqxat.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dlgetwbm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2irklbued.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2yxepyeuh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtbghutq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2igqlprzj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bkgvvumy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2bxhmlxpv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2bbyrnvxh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2tuwzmwgg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2slzwkhhy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hzwedgse.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uklldxoo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ccqhfndy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vmocameb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ewlihcwa.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bikbiohe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ccotktce.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2eyzzxfsm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ttiiiipw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2tdylepjx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ykhqkwon.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qdwlalnu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hntphcee.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2aaencrcu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2duqkzjei.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2junwaxvo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yzjdeaoa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nbvkkprc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qwiioabn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2sfzoarxg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2kpbexxhe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dhtlwhwt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xwqahnuw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2mnlvishy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lfxkqfsc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2yozdzxwn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dslswgrs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtfxpjfs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2hkcagqys.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2rcfvyxux.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kamcmchq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jffcnskh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ugphjvlc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vfnxdnka.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zayeaskb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkpmvuci.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ocvkpgld.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hmcwpqpb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yxaksvnv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jrrwgefv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ivkojjzc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dqkizodc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2xfsulrvc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tezoiyjo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2amwobjzf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zppgdacl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zutohrxy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2xzosqhxk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2svvnjwtd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2puogocwl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2solcwlfq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ocqhelww.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fpzlcrsj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zmlctibw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhgjxbwq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2zaoiqzkw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2txuoeeys.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2cfozgmjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjuicnyf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hkglmqhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znvdfuql.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vrnilssw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tkbjvshx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qusunjzo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2scvddkzy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2zjexsfim.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kfwdzkel.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2txazuqpc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2gvtkgrsg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2joqwtgkd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2beqkxpnt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mvjdxxct.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ofuhefyy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jmsyhrez.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hsforhvd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2snmhxtie.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2eeoiaqxi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ccjflxsl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gfuqdygm.html


<!-- 参考信息 -->