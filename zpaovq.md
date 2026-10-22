代发 wailian999

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qilrgtfd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2dlkbrmgb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2dixgrzsf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2goxlgmqi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ayicrthw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qblvtjnb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2fsidfxsr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qcpcfqre.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fwtqgtkl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2dacylktz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2kjsqzsdd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubpmruuh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kyuytarp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tmuocedx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fnfgaddq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2wezdhrdo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2eiiymoaq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jqlcczdd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2abdlkunu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2jmxmryrr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrrwxtmh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2blardmkz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivylknzf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zwposcum.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zlpaphhh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2roqaeluj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ooodptqf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wzwyepyf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2joyyzuls.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpgvbzvq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cjmutrpa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mpyoiima.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikfgdiar.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ubanzcbk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ezhfreyh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlkycgwq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qqkcrrhy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ljbfujcy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ivwwacjv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2izukerhd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qmzzmwng.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2nhynwaco.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qkbpttyw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2otqqxqvn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfgpbnrd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ntdvktue.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2gvuzlgyb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2pjvrewlu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2icmbquka.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykarxiif.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgeyahox.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2awejtyuv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uiigcrnv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2balinzeg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2cimjepen.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2exvitqeg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwidgqle.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2oilyauhb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiljefat.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gstwgtqh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ahxxnzal.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2cqjwdqxm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2axexydsx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2nuljzxcv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ftjnltsj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ggaronuv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ggagxezn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kfcuoiuk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rqueoxrp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lrfgssra.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2gniwzzqz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ncxkhyph.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vwlinrdw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2swyqjmdl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2maauxczc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdfqnxgo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kyyveyov.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2blgairge.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zelpytoa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rylnanwu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rixcnkdq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dntsilag.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2lkmifywm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2lucqkmaj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jvehggpt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lddzubpo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2sprukqkb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2usjtakgz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qqrgxdqe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2uoqmyyrq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2egnpiywb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2eijowtrb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2pbmitkie.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zjcziwxi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tnzekocx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vpsejbyr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2tstxiwdr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nfgxzdnq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2msfvpmhe.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cfnelsui.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fxtuxpii.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2uizobnml.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pwocldhd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2aquocaee.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qhmvukor.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ylsfqcqb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nsggwazq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vkbxxswj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zvokkuha.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2dyrcsrow.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2aoscohdv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtfnouws.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rldueqnt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2daxvjami.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2qnbczhou.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2rrlhqxkb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vwceagat.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2cldqxpqx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jnuetrus.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2edxhgacb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2goasbtst.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uklftxhe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jygcxoiq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wwvwydkg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ocmwrhwx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvatyfkg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2pptndkpp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ezssrlgh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2pgyrnaig.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qakqmavf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ynfqkfvb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xiprwipi.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hltyzoyk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gypbepuh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2snptobar.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2aqcdnrhx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2gohqqwda.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jciwujyr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tyvkiemy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2udqddfky.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ouvuvgkw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2itbmptgs.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2hfsiytfm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mrqpejsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzkwsctz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pgaaeqwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nznietjo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wooxphhl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lsajrcuc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wcuudylg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kggldjqw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xawdorsq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddswwaxx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2irwmulri.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gohgqazb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2owtutabw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2poydhxbx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2bposdnob.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2sipybrkf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dfhswjwf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xdjobvdl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ecitybii.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2cdrvupgp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2usuazkvu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2enjokpmt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jrkyqwyt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2wyqwngsu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2nnvtegyh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2aahuhpdj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nowkpfnb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vimutoek.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qcxeqsbr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jjqydyiw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vmcrseal.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jjkbrkxp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xtdrrxcg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vabnulix.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2funpvtgn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2iyqqxsuz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ecdwrpgf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dodztvkr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hlbkdwdt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfyibhee.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2dtfattmj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bgaeysyu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tjxkbmfd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2evlzmrym.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dyvqhwkd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jezjagia.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2iptjmbba.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rctleyzm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ghbbpnxl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2unfrkfvv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2aczkutsp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xftrdacq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qotriyqw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2laeccrnh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dxnogdst.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ghokrqda.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zxorasbe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dfltefex.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2opnjshoh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2cotvtjkd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wptvguzd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2udzqxqkq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2otfubwlc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jaajvohg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2iolcvzms.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vxzjfnjk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2cwxrbrmq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2dxtbhvnz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hhgtrorf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2vitsqhhe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxquqvde.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2flozxsbt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jyncjqvq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2pxcdjndb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mvhnbols.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2iovodoem.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2sallcekg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kkehoouj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ooqtlple.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fgsmfgwi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2marnstvx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpzaummb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2fxlivydc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvhrefaw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vhuiqeuq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2phaofott.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2dnwasgml.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2bonayndh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uczpzist.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zfigpnie.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sezzbrec.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wbgolosp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ynobqyvx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hsgjjdyi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ljefkjwy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vlqpsnin.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wggpjjpx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2uwhwcvdl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2dvffdaxo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bpzasewd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2lwctrohv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ooktxniu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2fnqomvfh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bepophsw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2daeqchgp.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2trrikvod.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sokgxyqh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lrfssssd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ltdaieub.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2odpmtnwx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rgmflgfw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2skhhmkmr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ksanornr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vzalwzbb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zudroair.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2shzvnxfl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgredyyi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ofixjelt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2glibpigb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xgxnhvzg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2usunmrco.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2nmtyhypj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2yydtibna.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ptmotoou.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hdmwtouy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehzlgrut.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ocntbcbl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wupkdsam.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qizkrwwr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2rwqublna.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2lxwsfdje.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ukomgeui.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hctdcmhl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gveigaam.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2covxulek.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mauvjshb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rgmjjrtp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2fhnsines.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pzuwkxyd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2uprrbqly.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fsujvoga.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ykxieapk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jedvvyft.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2npzfkzss.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2zdwbuker.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2bqgixeow.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rhuurviz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2wcddbwtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hldlhwne.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2mskgpkxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esrinsvu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rupddwru.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2plngapoq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wjbfqamy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2thklvyka.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2agolqufl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ujbgjfwo.html


<!-- 参考信息 -->