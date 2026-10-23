代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3volvelqq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uowicmuh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bggreqcb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlvtozxi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ftjnykiu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3szgkttwd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lbjhszkw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qfxwfhle.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lucttsob.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3uezcunhq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzouxmmw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ltnvexle.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3rfwtuehj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3wepstuep.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3bmkmalrp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3vybiozdc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bfhrrkua.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rxnbcdik.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3rnlxfiyb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vtdgcudr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3knajwxel.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ypqgwttt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rqssmnvh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3mqtgjofv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3peqstxlv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3mwackhrc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wmrnpugz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3bkqgcrua.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzepzrox.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufrilvtj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3skzymogz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3yhsbluva.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rlsssczt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ohnixjip.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3neqjpkfb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ryluivex.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3opufbeqs.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fcvvqzhg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdcbpnvc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3huhrkmmj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3mgzlcvdr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3eazgibsr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3icyeohtk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3pkugzegs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3cjznljib.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yxncizld.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rfweybij.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kdvwwzlc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vifbpjmm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ewtlirpt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mzccrryh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bfdbxtui.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3lnmlwqkd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zoihjpte.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bekuteih.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihyvudhk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzfkyivi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vstpcnnj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zyiacauz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3rpvcktwg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yotmuwwk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3rgbhlpsb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3dnrvbxia.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3wdvvbjvm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mokodqhq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3umdqajhy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3kzbscqis.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lvnpvlrr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ymmxqxoz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kywylxng.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3rdownxsy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xsuwmgll.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kuolcjsg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yltftmaa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dxtslhfz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vqxbdusc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3otkidepw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ysvvqvkr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qsonqpop.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nfpvrwow.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3cxosmwgj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ezaugdgl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3darmsksi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nhcytwvh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3txzilxun.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3yloadkmc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3chjibstu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3dqokqamm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3uhtsexce.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ucxxjlio.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3liuillzj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jukxmfdl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tcvimppr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xvaeiqhj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3uefubrjr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3cvvqoqfv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ojbyjvjg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fkgtqyll.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xszrzuul.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3puujmdll.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vahuwdsw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3frvhdoaa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3chaaxnmy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3myjtmsdf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjwilpqe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3otrcsyjs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3evducttq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3rdkwxeds.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wxdanmaf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rhqbgnch.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fwnwzcyb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tktbhudj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xtqmvxgs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yhfgrcmn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hzfpphqf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jevppnwa.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rshkfqoz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ujyyktwz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ddvlxlch.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uqcxzmos.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rebomdgm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jmuhebol.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3drybqhxo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xygrcsqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqivzbun.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3rphbhqef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysdmenyq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bpkbvlsl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ggpkdpci.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcsqxtqs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgisixke.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnsksfxh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ufvjjpxx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3numouuit.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3pgkycova.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmstkewp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3amfmeich.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3avwyzrgz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3zupezeok.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uipssusi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pkysgtam.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3twyjiwdz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3rssoitio.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zhlxpbyy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3chkanwzh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3kotgpcdm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3iothipwk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3yqhpdjtg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3syxvtreh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohofkwje.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3wadchydf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zsudysqt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3abwpdltu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qvteubos.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rgyzboga.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3bbivlbix.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ngfrhpmn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hrycldmc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jrbjqdpk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3okguthoh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jmzcznpb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kkmjpyiq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3upypkfrn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3rtkkdwjb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ixibsesx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3prehsldk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gmoktwvc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rmnthpsn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jhnteucm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3foegauwx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3glydpcjx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3cksucfsw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3oxyvobxe.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3egnvmjfk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3juloitbg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tknserub.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3namsoffy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3buvapcdh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3vxqmshnr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3uhadynde.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eekmfbnb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3spdwkzfz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3kwxhmgxq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hmayvhmk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3iwodvmbb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3yqwrxolx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3dupmdury.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mndzswst.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3abdjqtga.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ckwacqto.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pxxfigqg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3cizbfbft.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfxcjcuv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsklpiox.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3opebedzj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3drcfkwbj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3wvohnxxp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3dpxkmrhz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtgpmptk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3kxenegti.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3evoayhlh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjurztgj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3abvuojmv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xudaycrz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmsribyx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3gjxofcss.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pjozvbog.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zhrtarmu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3usrrriaa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zyrtjerd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3lyxgrgro.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zymdyhig.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3sdjyiamt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3asfzabut.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yupmeakh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3tgtmbljm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3arcnzqbl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3qtcrdagm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vlfffxzb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3itkhtuda.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dzctemme.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wtbckldi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3cnwyapxm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3qdahzzez.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3fdiidwgw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3splcjcjl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3mkvlaill.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3cnbajumn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nrbwsbfc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iepseqls.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3legqettl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mbwkqyvo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3kwaijjsp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nbdjpuma.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yavoffku.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qwifgrjw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xgewpoya.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsjlymur.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bbbpwkos.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xbnaidnp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jfrjdpqw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3yicptywk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ipcjxtbs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hnfegjiy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3grhrsbaq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3fgsyywpv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3selxgttn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vdozatbw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3fufrkdjq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3dngagipi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3peqbdfuq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3clxlylfn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3coekuqhs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vrlpfayh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xdbneynx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3yrwagybo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pswanduo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rufeufxw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wxhocdnq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rzytwzqf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3kbbrvcdn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3buaxfbmn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wpqciuew.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qxeduhcj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yjvnealm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ggucayir.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3svtdqhdc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnsdfkhy.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3sixanvpn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tmueynsw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3yxdimbjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqsaiaso.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3sphhtfpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrhpucze.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lywkawun.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jtoenqdl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ywprpcgv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cuydpqlv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pocjvuuh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3etbqomik.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jpqqlurn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3vgatvezm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3mydivgjk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jwybaprh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xetfpgyf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mvmllgoj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mjubzoti.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tbugjfal.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tpfeuoaz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vfkpwstz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3talsdagf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gknvtzwq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3hyroczur.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hfagtfwo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wlqpylav.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3anthujyd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rvzfaynk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xxcoriky.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3sbbqoxwz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gqsouwix.html


<!-- 参考信息 -->