代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ggremjqh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2clfewpmt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uxrhgthd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2knyxsqhq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zhwnvyqq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rkehynar.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tuwhowpq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xmluilyk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2cjxpfuwb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kdsormxn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2vyaegiia.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2grpnjqsk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnpegdvw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sbwzdgeo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlmwhnqh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlosbbdd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bqltmplf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zroxhxgn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2eudresdi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ckfwqlfn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2oettbosv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2tvevygjx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2chiltgqj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wheknqjs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ruteuldv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ravbzzpx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2vgsvrrij.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2dkqldihb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lthtygin.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2dwuxjygr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2zsnioppq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cifjsded.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cgtlcdqw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2phxwrmcf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2uyfnswjr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2mgrvhqwq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rxlvdcdf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jgygdwre.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2heyrxdqk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2drpcltcl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqsojycw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rflimgsl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xxoriezz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2aefifdfy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rrhfimsm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xzgauqgy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2alizyxrh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qepynkvr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywmeutwu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mztefgef.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xyplifor.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mjzublcu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2pdtopvwo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2nijyscsl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltseedim.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2novoikkh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wqjevwwy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ghfvlddj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gkyihnxq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2btuhxneo.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jcsanhct.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mskdyrjo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2utofmcan.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qrecryez.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wmcbbcxz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2alwhbrbt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpgpheqs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2thyizirh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbbctyzt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfhcwrlm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jyxnnatw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2uhyayxcl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xockquav.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ywhogkgc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ikvlqsjh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdinajns.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2skwpygox.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wbslphdt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2fhqscyos.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wvjooywp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2umbwwwiu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2niloyyym.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2pufxlgku.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2sgwcbnno.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2bucckgzl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nagkects.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rweybwbk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2itzysvoh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2fnjdoojw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ktrvmnxt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2munpzgjx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2pmoxamvx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2etllwuxh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2yobgflsn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pvqjrvhv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tasujgtq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2glohmxhf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cqkeusfa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qrnnsjit.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2mkjlgfoa.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ljeleaxi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2wszxzirn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2yizbueee.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mrrvnszr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vzujskbx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gfkafyrt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lergxroa.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ussvwtyb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2iuduquod.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2oaywinme.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qhbmxuzv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2cgigkwro.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jjiisgkw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gqayhrqy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pbeoevfv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sepwclxw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jyxfnxjq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xmfakbha.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fczvzllf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2hrrklhpa.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2kajzudrm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2derbwbyh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vvcdvqca.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uotwbwnt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2abpqkoqg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2euvyahna.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lhmhvbja.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2cehulxms.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2eekphogg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqhplsjc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fhnyatem.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hhsaqlfz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2olbrlxqm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zkuzehio.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2bxocjibt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hemrxbtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzcqeard.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wdkcsfad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdajzdnf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mywrvovh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2axagpfee.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yyrphdzw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yutsqtnw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtfvftrt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jwcctlnr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jkakbadg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2qarcriha.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2imbubmfo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zkdtasvp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2auekxaqa.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2utwvkhgo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sumbzyuo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlwkrewh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hchxaupx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2rlprwoii.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2midamuzm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2uffdrxnd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2yceytqcl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2feujkadv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2sfxicqjc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaqmrmru.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tenxteii.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2grcxuntv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2xbeujayg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tyhkdxqa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2tdbudfui.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tvezbvmk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2txcwebkj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2sdkncydu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qdedfjbl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zqwsjitg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2lxddhukb.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ruenrfyj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nrwcuywk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hbfnvetj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2pqwfylfe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pxpxmbcv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ttzejbtq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2befpftbo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zpfgunsg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2zvtzzldl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lgstfyat.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cbokaovw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ctbfjkpn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jwejlrmx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qnsdepps.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rodwtdzs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yshwhexz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tzieppkj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mqbegkrt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ryucvjxb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2estouifh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2voflietg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2xrtvufso.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zpzqxhjw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2neqcauop.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2odqbkglj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gxqzccpk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jqfmhwle.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rqgzdqgr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2nxwfukho.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hkpupljz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2fzfglwrt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2jkxefocr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2oggvauho.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vdwskdwn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jrgldpkv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vazcwuxj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zrqwdomy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2csziosgr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2naweanuv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2huqoktbw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2prbmfbqw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lyodoecw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ikwsrfqe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cyjharnd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yusyyxal.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qljghzsk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oathsyqc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2tipsdduw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xgfzqmny.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zdacjjhm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nxlisabo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2jxohlmsi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jtpmeivq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uthiedgz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qjewaeim.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pocytpdt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2itjkmwcv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2cdcrpauy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2haadvacx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xuebcvqo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fvijephp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2uhoxghbv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wrdeqefz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kqcyducz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vfuryqml.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ojohfrfd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zvdmryhm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2njgmzpwn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ljyrftwr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lhhyvatf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bjwgadvr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2tzquembt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2barklpyr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qjidbdwk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2bfiwymgv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2sfmghtkk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cpoqijkd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgxsiiuz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2kesgmitn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aiqldneu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxstrsez.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2fjzfczbz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xepisntz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2oqpcotii.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2mrxlnxlj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wpwcsufp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rsosklni.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2szebjfck.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2huurbbay.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vooqkubb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2sewuqmtj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2logxccre.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gseuwxde.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2exhbndld.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xauomfpp.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fluykeji.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bpmgpaju.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2duszebih.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2aikwksiq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2boicwhua.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2pwlxoezw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tdydxkuo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lbcblewq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ftkmwnrp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rudufeso.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2rvmlswut.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2punohjjw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2rolymkkl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2yckxytnr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qvamaytu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2iqclpxxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tadgpbxs.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nzpuoxcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kaopzsfq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jduparqr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tizpbtcc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jktznwxl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2glktnisc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vhvdjipb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ohwozjbp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2iygyachz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2edcijnfg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2kneldoze.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mdkxrckh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2uwvmmjyi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2txtuintk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nbydjyug.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ruuaxygc.html


<!-- 参考信息 -->