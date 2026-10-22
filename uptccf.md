代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nttvxupj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2trvwpfkw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2vpayojtm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2htnpqksz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fqviavod.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2taquqpyz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rpyzjjip.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ehpwxpzn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2sxufacwk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hponfrur.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2phnthdcp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qztihpwm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2xqpxmtek.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2mchvxpaw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgsxdhyz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tfcxgmjd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ybwjjhim.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vhmkwgnh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2dpbdsuaz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ekqgykxy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sdockpmx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ofjlujjf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2bimdriva.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdfkounl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oefizddi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2jtwskdoh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dhrexgis.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2eyfjcsxb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzfcdihm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gpahtsgh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nebeojes.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2largabdh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnxlmiww.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgawpdsd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2soelggce.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nvdlfwsj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2snlatymi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfhrbbsm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2aktsqvgh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2trwneuud.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2fwlxwuyd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dbpjgedj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lxbuxszz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mvznylki.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2yayohgmd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2uxecijes.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2unhaixtg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2aqcdqnkn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ozlrxrhv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zhubqphf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jlpldejo.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dnjnqosa.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dpbpefbu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vmzedlbn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vysbjpkn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2trxxxdod.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2fuhpgjzg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2knboiukz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sweedknj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdorukni.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iudijhzo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iruysguk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ardlaqpp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2iyfvfskl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfnoxats.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dmfmcqol.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lyqsatzc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cazseote.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ymocxgkf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rfrbxymj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2qjrrglov.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2mlsglife.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cxcnopki.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymilhlep.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2coykkgph.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2cybndlns.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lflchoat.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2czfixzze.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ogfslxnf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2jzmfzcrd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xvdljxzr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rxbfjjbk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2lbtlvido.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2oinwkvtk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2bqhmfbcc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ltmalvaf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cbkavrez.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yzblhkcc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sayfbxbl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rymdebaz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zcxllnxa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ohubsgwg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2kzrzhzlk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2lttlupee.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ibpsgteb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tojcljni.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcihcldb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qbyhufod.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2kvhjnufa.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2spxbmokd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2foroenak.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ueuhkils.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rdnxwjkr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2fbsqprnt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2albpnjgy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2unsgwxlq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2isuugcdx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rvkbxvog.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fsyyuevw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pvpbincy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2dzyxkrxz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zvlyhmre.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ugdcqyyd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yylgeubk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bvrrxyux.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vbjestie.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ttwwpghg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ncrcsdla.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rjnremnj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2haltosnc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2fbxqvtst.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rfqyiimt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lqqolfdt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2smzqhbbd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hmacivfm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ynjlklqi.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2mikettcq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gkvvosef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnzulief.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zrqpmzkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlcdkdrw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2njcmuqzc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zuokfgsy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2itljnkzh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uslikzoy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lumblykz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fswvexbc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uswavbon.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2drjrnkmf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xarlselc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vqyexmvc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2xcnoqptf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dqfnwncc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ffxsbnmi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahgarucp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2iqniyvts.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ewohshye.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xbmkbwbf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2wufkzvhx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rrkmzxjk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2pryzapag.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2limpmlrh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xwyyaael.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mujggkkc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgiywjqc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2cjluorkh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mtdqlxbx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2iofwefdz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2syakvmfj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2eeyxdbxf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tctggudr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vqpxsvjs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yugmuoiz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2cxirqnpk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2qdzhlzyg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qfwfmfgl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ynzchyjc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2esvcxesg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2igjtmies.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2brbugoer.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2aqxktftn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2frortigq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2abbvlmtr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rjnaxatc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2orafreyl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2dsngvwey.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2axrhenjb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2dgmsajnh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ngjkdchu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2khsfhtxy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xetvyuoh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tdqdlkiu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2barzrfuw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fjtwxwtc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ndpleqpt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bgbctypq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2qnaqedcq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nxaltaga.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2jmysciqz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zinhlwkb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2guwrhlft.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2gmbexddl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2baqfkvfx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ennltzzf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fxyjrxlb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ndafwlov.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2twtoygxa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iblergfv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2izynpnmb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2kzqdobxg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2lmqdxdqq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2skvsppsu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ccogyevw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fcotjbpw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jjiktoyw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pdzzsgui.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fffboosw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gliwtxrv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxtofnrq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2peipsebm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2crbvkqnt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2omwwzlta.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2wnjzukbq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2fpghmczs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ygbwxcye.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2simkcmdw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2sctxylqs.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lhjvimel.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vedejzcj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2mivdqnlb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2asqquelg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2dpstrlyh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2mtdfjycq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tsxqmgcy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fuwlvufs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wjmnpqqm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ujuuxvvp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qbsgzekc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2cokuhcrt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zcbhcrbm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jwbrfail.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2syfqxemw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2xxlebqrz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tmurgdch.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rbnzbpxn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2lidtyzgc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vzydrlxq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dyedgwxv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjxeapbh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wvinqnpl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jixsqjda.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewvfmlhl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jhzlnbfh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwetothd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yksiypit.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dkthubje.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2rshcsuqn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2fvhzubqb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2gpfyqgxf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lrioaytm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jfvzruqu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dddlcjhs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2cjhrpdrd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2egeydxyj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wqkyzdbs.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2oirugmmk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2kbjfviij.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2eyvbzwzj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2jxicdfoy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uechaldb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfrnmgbk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kpgmxpmv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2onqqfwum.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zmvqsfea.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2frkudpqb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qvtqxyvm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xprwjpoq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jdqqrdxc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tbwmdzxm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fbdtlciv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2oytbutdc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2uvwmnhrc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ztpcofpn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lfojuydr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppymkqst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wntfqlew.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hlrbhcrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fktlwlol.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kisfpjxc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2djwwqwmw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zdjweija.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qtgdltkp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2nprmvftd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2cjaagujm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dirrcpro.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2bvxyopfe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2htmyyage.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2uarxszxu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ilozuklm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2twphumgk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bvcojytv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rjwjyvob.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xzyfhbqm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2awgmyzrb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2djhckqpz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pwcgrqho.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2vkpvgwss.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xlblzjxn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wdwwchkl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2crtoxyax.html


<!-- 参考信息 -->