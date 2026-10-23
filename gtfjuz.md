代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eqtkshwc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ktqcyykg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3bhdhyoby.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3qecutsbr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rxyjyvcr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3alnsbpuh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hvanstga.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vlaoiilo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ngerpkml.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vfbmxztj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wapuzrdp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3uqgbfrxt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qkinhgxb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmymnpwx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3antdfxyb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zmkmgdwz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3elinhruo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3eblmnlux.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3latcgdgt.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tyxfsfxu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lumoeqir.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3eanumjpi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pohclddf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wtiysbjn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwkchiav.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3eyuwdxvw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ugnaatna.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ebsedehh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dzygrpkv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3lnsyvaov.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3uexklpyu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pisjtwbt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3evhqnytn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dulnbmyc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3kwvumwvo.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3fjcozdzk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwfrtepg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3rfglptwv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wjlqdmtg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gszreilr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fndbswnj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3isideclt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pmekintm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3uuruhfwr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3qqakkdkj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzxkxxvy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ggmjdjai.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qeexnkkl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yudvntsf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qwqnlvki.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3clqqgmhx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wrdqazzz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3dkpsmuif.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3knkmtrdi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhennnjs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3khhvtrlt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ajvrjpdc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fmlenhdf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qypwvqqk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zylzethi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vwzyatwk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fmxdclcm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3adtfswit.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iuapmxbr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3bqwiocbp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jgoppxif.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xahfjviv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvxqckqp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3txdaafgw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aahojbzg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ndmbnoul.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3histqsdf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngtgasqk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xryktllo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3hpkhrqrc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnulqcua.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hywnuyqo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zdxkfxpp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3isxhgtfj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3sdbncgkl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3saqxbjjj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsnbpmwj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nddirkdd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3aixrixsp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ooyybjos.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kzcbwoxe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xdnpjopb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xubvoudr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3tctngwad.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3glyxxiws.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jwbucyor.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3pzdukniz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ozotxlzv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3pbxoaxjp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mtzpnzem.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3htbgifkk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iwkcdcij.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3vqwcrcgo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hetgpcdp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3fidsgeyo.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3hcxhtyuv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3cbsyemxb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymggceac.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ggzkwvbq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urnvewvt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ktjlhgkm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3kuewwzce.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gdgnxsst.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3zizsxhpp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fybaywfo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jiaysrfq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3bwtzyape.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmnlujcc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uvsrpxyb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzzknudl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3fmruhuum.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxctwmpr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ccqairaj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3stsnekaw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3kzsjsebt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3aqwnkanw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ykbocpvv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wxzkqade.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zfecsfwi.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3igjhesfh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ovtvlesl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3esvxhevo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zyuletwr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ozrrfjia.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3pnjwyyxb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zybabvpz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zacgkcmn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gwiwxnka.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3xlnzrefv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3yfojpaax.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zlheusjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbucdezp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wxninmlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htdvxkhz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jaeglfki.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jxfzdage.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hkczeadq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyyecrnl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hybbziwn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkfbiwyd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vghkhqvu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vkfycjes.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bgsmcvvs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jgnyhxwr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ircmsinx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3udfmixzb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fjkqvdsb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hkuxpbow.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3jowdhesg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fcqpnwof.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ohnjjyim.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3dpjduhod.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ikdwxvyi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3thvrrzrz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3skxrdgrs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdssxbzg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvunclmb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vqkwqqwp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qrcxnafq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gedabgsx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3wpbfaqkj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3pdotcmwp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mdertvkg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3evgxbyhi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hqgjkgvp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rprgniyn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ptrjwmel.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qewmzmqk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwdurrkj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgabfybd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3vdkjsvkw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pqngvyos.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nzogmejj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zyiwhqmb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tcytjtug.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3xfwaijcu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mjyuztkx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3otxozkxy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lbsejlbo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hsvcyglk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3tueriekr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zqlevaqx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dpdxgfea.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xteifmyb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3lkswlybw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mubnzidi.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3nlgmajxe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ciboyjqa.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pyenzumz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3jeckfnvj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pjctpmdk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3lwwfyhib.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rduvssku.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kswqcfcd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vwbqrjft.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dewbezlr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3seacxxvx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vwvxgebe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3yeixlbbe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtzcumxf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcmjzkik.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfffwqjc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3gdvhedlt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3edeppgmu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xflljtbb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jxttzltm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3cpzwthvd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3uqzjkiwj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hmqdrqjl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cjmzhxuh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mmdlwvuw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwjwsggd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3thrfggin.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lgdzdvpu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hiypwobh.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lhhjqrqp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3rzvqiefl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3qsdrvsll.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lgjukhpj.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rskxrdmh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3iwcmedlm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ypfpdhkc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3cvpkobpp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3amlcuxee.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3uzbbdcix.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3gmkfauwj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3yijwzkhi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3beiijswn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3bacemzmj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fuwlgjpf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bqobwrvw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3qouswkwr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3bjpnwvmz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wrdlzctj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3gqweewnm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3uuodxkwm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gxjqhcax.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3alqoejxa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3itolhcwv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wnvwimwe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3iwwjeieh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3nknlsgtk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3efykixyc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3issgnmwg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdecrlig.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3mezpbvlv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nhgyeodw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3btgwvunb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3prvnrtbg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ngcqtrba.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3uyoteaov.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmeftmwt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3qtlayqou.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dudixjnx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ijjlpfsx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ismxjfah.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukeneagd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3lqqwmjxl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lssenkze.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3stvssoph.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rnedzhmc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3oiuggnvl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wlzgcoel.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hstzwcps.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fptakmfe.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tzvvfvkl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hxxwqmaj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3nhqyjlbk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3broosbwl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qnttkvgp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mlmfoljf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3nmrninnf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3vuyqdpmm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ploonwtu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3phqwsikb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tbjvfhhg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3seklwhzl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iyeqvbnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tfgfeehf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3cljhyyin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcbcvxvv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3myofabqg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dmmgjfgw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ynpgsuru.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vifbuqvw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3oasuvily.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3czjrpgnn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3fjcrrhjl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ztepmjej.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kgccfbbt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3oualjopu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3dzqnagpc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3apremysh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xfgbfunj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rzkoonov.html


<!-- 参考信息 -->