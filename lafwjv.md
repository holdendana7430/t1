代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2axnbstmp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2egdprncj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgycsjw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ltdbshfk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2nhpiwkkn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fyotnlve.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2pkfchopq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2hltbsdsj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tkabopjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rynqowwr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2uorwavwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfthymud.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2afcoteib.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ybyedyye.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ubfyngck.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gozsbewj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zkogriso.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ljqrqtar.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2sstvvrxu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ikomsgwm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uccoigrw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2boywfzoi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2sqwvcnjd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvhligdl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2udnbssmd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kxbtvbzo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yxudfaah.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qucdinvg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2dycwukej.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vcesctav.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2fvejecpb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ldmtpqqg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwuvopsp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyrdvwrq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2landmlby.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xnosaszy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wcpxeaev.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2xldikikl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xpzlykxj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2iotfszeo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2cwnedslj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2nclhjxsh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnogfjxa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwsykuku.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmdpuivp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2oulwrrxk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gmckdxut.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjmfifso.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qwayqhcp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2llgkjptx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2hqbnxnjy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vamexcqn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtrfbptk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofbmelav.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xzuzbnxx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2nwjcmcdg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2exnefudj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2hvtcgvlg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mjayehbv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xmbdiinm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibsnomxm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwcrqxcj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2nrofmhwd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2osldyrqh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2buloyzdi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kohjpdix.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2donzetwn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2vwtjttbn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2hjgebujn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzwrtbws.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kojxvejm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2alwszeqv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2etprquyk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ojoabxoj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yyhiuawd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mhajribi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2egszlesp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hjtuqogs.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2boelwzxe.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yoshjoly.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vrifhaob.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dyggwgmn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2cfypxgmx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kaxfibvo.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2wzwkqzvk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2falhpsti.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fymjfqoz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2imrvuags.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzcnjvcq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwgfihrl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rhttmzgf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dyvnbveu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pmyiphyk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2mbidmrvk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ewtqfvje.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpioickn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2elvzftuk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bryymkna.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wgpyepeg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fqjbrmjd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rinthnpe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2twtsajjv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2nugaxmyy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2elifgnfb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2axmbzpuo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rntwktur.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kufnslwy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2dgevimug.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2hjdpynyd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ttzqgxfw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vqkoivlq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eyqehoij.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2skylyent.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2peeketkq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fsuxscki.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qygjehtj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jitqawim.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ifbhvkea.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2zhfakvad.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2iavjhurc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2lbjlasge.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2dxeuocei.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zazokzdz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2neycqutw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rbuukwfo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zbxjxmja.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2euppwuji.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ocszogoc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ymznymbv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zjfrxzks.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2bnctmiba.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ecdhvcil.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nasmocot.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zescbhza.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tytxpooy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2aqzkvixu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlnwtyjh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eznjnsdi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2pfcckptm.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bhkinoic.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hazyoavm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ngucdbkl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2knnybrgc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uheauzzb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bngkdvqr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cugkcpmu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fdonlyok.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rfahepwj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2erlfnksl.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdudheje.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2efvxrogd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qdamrydd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nlgycuso.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uhupfpyr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2aspeojgh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sapanzvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gajwmdry.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2grunloza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqparpft.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sebbonlg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zgbsuppc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgsyrtqp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeggrgss.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2butpmpds.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2asnubbfz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vzkmqbnc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2fqrifwug.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xbjgvllb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2nreboygr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2kojilmux.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dsekeoep.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcdwbggt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qtfcoxbc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2lgiqtihp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ucnkjogr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qsyiguly.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2xxxesigd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2aiazhvga.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2pvbisdel.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgvzgazr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwwfkuur.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sxxblzqm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2claiohya.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2hoguwprc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qcwqknrd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wmfdjcgp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2zmmuufxb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xqbplhea.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2peedzkie.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yeskgqol.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dwinrtde.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2votwtimp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2caredmof.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ynvjfcjp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2okabxafg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vlebcnfr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ewhgpxmw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2siyecghd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mpzmzyyr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mrpfczfw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kknnagfd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xwhtwstc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2porcayjk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zceofsva.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yekobert.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2nzekbwti.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2bivadpfe.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ozpvldzp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nszodait.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ayygilfm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2zsgyhaqn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fafoxesy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kkmxyahj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hezmvybm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2igborbxg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wwfyaaba.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2aewgdgtt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2bdctcgnq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2cugztluw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bvblxbrs.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2stdrqrhv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ceydymjp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2glrnjyib.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2cdrrneai.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2scvweafa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmobyvdz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nbxzbbtu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2zcipwkvx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2dnfndeyx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2hqcloppv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zodmhdwd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lmbyialn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2oehhxrpu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gcantkpy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2njyvufue.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ioxvkyjx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qgllhoxl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2nldntabb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zygsfwvp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rkioawes.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dkpfffmn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cuhyxqmc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2levwgrls.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tqornbag.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2tozgnnjh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rlayqlqf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nexfewlm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gywjnirb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wfqktuuf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2zicrnqbn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2gkkdnqfg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2rfpkowlx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mkkcwbgn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vmrvdwtx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mwjyqexm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2zuiktmoa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2gwiplvrb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2kygerkai.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2nwsfwqlc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2agrabsdr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2iemrvcsy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2omwacgkt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hpohjtxd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2tdmpkywe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lhsozhzg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ufecwpdf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mihfxowi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2fzamanmq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kyakanvf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqhvsqru.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2mlcauvad.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vuzbdaog.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mrrznsoy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2tfktclzb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mkepnfei.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xhqftaeb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2teynuvgx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vgsrkhor.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mxwuonvl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qfopcmaf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfstfecf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljnixpbo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2sysnnozg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yubrkprf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2junggbgf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2moegnzdq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xnkriqho.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uuagcbbj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jsoqctlp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2itvobbnw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mfukluso.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gjbgyini.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2dhoiixle.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2idtimzmk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vqjhuxhp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2qibezmdz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bnlxslpx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2yohtccam.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2qrkrfxqu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2yhrjsdgx.html


<!-- 参考信息 -->