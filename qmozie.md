代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sloikffy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cnvjqssd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nlouugin.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2bvpwsrep.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2orosofee.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2thinlmjx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2tqxnetqq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2mnwcslva.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqpgqvpe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2taixfcjq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydumgybi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfvigsna.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zzztwktt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2pghhtiwi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hcmaoxkb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qsrrrwze.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jgigghvh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbzrlobr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cujrjnhj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gtpdergr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xtvwfqqp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2stmzxauk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2qweihxfx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2eibsjebd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nxumxrbn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2vdkzzgjw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxlwdjtq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjfnyqat.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkqccejl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2kixbxrdq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2owrsflfq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2wjalyacb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2loryzmhn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2lbuwaxgh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jazabzgm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmjghuha.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2psvpsoql.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ucronxpy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wyfltwed.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2cbzlvacx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ejejncap.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jieuhyhf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2dwzyqxhp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2gjimqijy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeaggisg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pvplnfjr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dshwtlaj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pdnxbopw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nlaxwphd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bfpldxqr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgitwqyf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2tdyrvynb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2txyqgznd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gatzxukx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kxwthpbg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2glftllwp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zrpgjdpi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xtiqzvfu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jxmbouke.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2izqtnqnj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wwppqpmj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2nthxihdt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbvmyvxd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxdbibsl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ehzrbnpi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jfokiobs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qanbzkrc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tpxoqaxi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oweswoby.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vglsqiet.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2qmmcvstd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsedcmny.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cwukzscb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ytyolgfh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2dasevahi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xbjughlp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pwpgzazk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2olnzajlf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2dpqiojov.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2wlbmonlk.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ovydlpuo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2erwedqsk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jeqievnn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ravgvwqq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ylkeeapp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uogopimj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qfzgperh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kuobeoed.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2rffdrnad.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zcudjqmg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eaxihpdq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pvyhndyo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mrsnonpp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zlnkiiwm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2gphdvnpw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gskchfpc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wwebwrpx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2fbostgyp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mcvdyvhn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uxgvthpz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jefuxrxm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jnfbbtib.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2btyrhudw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gjbgyglv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2jdvgwstl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dbhnlnbq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hazptiwc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rdpbhrjo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vtadzfbr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2prqtwlff.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uklnzcwl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2qtkaqeql.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2spyxamey.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xxkuaier.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jjyxpkhp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2neyhmsxx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ccxuklxk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nhurkesu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2poweskww.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2spvghmaw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gtspoopi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hgtvcirx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hwersfai.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rxyceqao.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jjuxdqvu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvddewjh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tgmejzrv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ohhlnvgd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tjaeiopi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2zylqwegb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2cxpbmnzl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kfyjgudu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgwqykst.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2vrjsdnds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsfreptv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ylbubswh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2swcruuwf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2csygjvbh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bjiuqccn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fhfglsfu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zddhbpjk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2bahtrybq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rxjzrxop.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qmeevmyy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2vxahrmrj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bgdypfqh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2yvduexoj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2edkhbscz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxbvawwn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2asmnfbfb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zmoepwyo.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2bqvzdgns.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rckvucjq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2itzkhzns.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2kifmukkw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ehcatwdn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lktomkcf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2olyjpavi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2yeboxsqx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2bfoeeqgo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2dhizabkb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2joozkoog.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2nbjlzxbx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2hflphgmj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cdiksqsb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axfavpde.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jixbmesr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2diqybkvw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qokjwgox.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojfltjbi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lxtyxhwz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2wlgdqqvz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yohlswuz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2rlwbepnd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wygasdus.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nymrahoj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2bijguftz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mxwgakqr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2btfzzvlx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2rlgovubn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vzzwbedv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2sbciwbjt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2nzjuwulm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jaeffbxp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fmwacxyw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jlxcpqba.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qlrpkynz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vlxjzhih.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fdakwekr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pddsmzbn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2amwqdvhe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kkzrpime.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2kqnbnsft.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ztwkfwyy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jdvwekfs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xopvengl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tshwgkgs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vzznljea.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ehqdgaci.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2buuriaxy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nveyqast.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jalbbppc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wumcylpa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mvuoguta.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2woqwbhah.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2tbrymxng.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkgoeqld.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2euamtfwi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tyeigtrr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzxurumb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kqotofal.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wgbwytuh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkazmpgh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qdljvozp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rihhlekt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mqyrsozp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2pyoeljnh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2lwkrtnyb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2avmctjfg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qrduuobl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2zjiirkmj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oagmlggv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2docsyrkx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ohoonyto.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mktpqklb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gptplzjs.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kliraoye.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2eeyovhhg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2etlmjykw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xkmioucd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2tyisvmwq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ftufebra.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vouhxsby.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2nsnufxco.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2kyawdjdl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lgihknku.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2acheeyoy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nawujter.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xtnpbhan.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2sjfyaeot.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2maumnuiq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rqhikpny.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xamgsojj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2reftywqc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2uofokupz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvueeihs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2pkvkxkvj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvdjghmx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmvewydg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2nzdrxqae.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zmltsmmb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2rcsgxylw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2yxggjilq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ujspagum.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lozhjtgb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gjcysffn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgqpgpfw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2alwlmzyb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ijjwiqha.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tqhjcspx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2mwkzapzh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2cqhfadva.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rgsmlofm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2evsgidct.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvlyizch.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgyghndo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wbgvxiyz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uwblfsmw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ojhxwjwb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2olwofgtg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2jhherrhn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rbpettnf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2aodctahk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ijmabpup.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dgjhwgim.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kptizlxs.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cazntcwm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lhmlbhqq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbkagexx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuvacfpj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2gtztzpmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzsiywow.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hlukczpr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2aftpbwtw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2aroeaqvc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uzxwfeci.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ysqqnqff.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2prsiyiek.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ecmneulf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ycgqqvnh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2uqlqthjq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2rwdtevpv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hkawvily.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ncuwaucq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ufywcmwu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lcqotvvg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vntwszyi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2akvssfcw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2dwfuwkgj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2udgowcwa.html


<!-- 参考信息 -->