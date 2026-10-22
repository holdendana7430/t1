代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2uwwqiupv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcbptdwe.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2sfkkfdcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elwpyuhs.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2aeoxrgzv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2uyzutiyu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ysfjlkvf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yldschih.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cnopobhb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rcrizoph.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2cyozirbj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fwrodyxt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sagmhaux.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2dkujtzhw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xpuapizg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nlpcriln.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tzpimnnf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iiolgsfq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2alltgjlf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2danxozga.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2vzutscuf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ereevxwj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2iusztudp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cxqvxosz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pgolzrsp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2heqfchzg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gilxeftq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2acxpqaxd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2saatntpn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2twbnawji.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2uwtufgjx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ihmlcsjx.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jewlwniw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2kchcwkxp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kyfbqfin.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xryljieb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2djsockau.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2jdgjutwz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2shxtcijq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2tswqiucj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dnpztnfu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ahjxajhd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ojzslgwx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpkszrbn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bmbciijk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ivwswkmi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2fnctvcpr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2gpztapns.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2kzpfgzyx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2yrepzztj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2adaahodb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hwswfsbi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cuibuewv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrglfwjj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dodrffcv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2htzgfpzw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2uhnvnjoy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2oiuytcij.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2cwerwyuf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hnnccqpi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2lcikhznj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xldohxeu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhxzoihw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpworukd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2mnzrrkse.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2uhlsdqrv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jrewzyml.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2fiavsuwg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2vvfimmpw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xwtgmldm.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ustujcew.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mfbpylse.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zokrkcsx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uxotfakn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zxhkwqrq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ngeehsxk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2gffzqifc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ordktxzc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehpbqvgz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xvyydltd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aauwyhrw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtlxvlpx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xrwyesdp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2piqidqva.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kltyzoti.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2qvspnnje.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2kklpnpdp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqzrjpsy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2glovmlbj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2aafmxltd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjpyctzc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kzsvdztr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kowrwudw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rhlpyaux.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2omgnzphg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2lgqgtvnd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vcflhybn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2slcqexqm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qnsslgky.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xgejtsrw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gzczoerd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2lgsrznuz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jrgrdcin.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vccwyher.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2egivojza.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hyjrhesg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jkxsjafi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hsrrotam.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kdaeiiyd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2kygqtbbh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wcuwosnl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2fjggyhru.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wjeakqym.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vqezshej.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2frirzmgy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jyynashb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nqxhhldx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ebanvcuw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ngiwaarm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2dyvdwabk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2enjhhyax.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2bmjakqts.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2fhlxowxj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2crsuacgl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbhtlnoi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2viqnxwes.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlbtvfpy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hkizcobe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cgqgapfw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hwepdeum.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2flknxabl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2gcueuywd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2qtaimrds.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ekfxazfg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tyirgfni.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ihqeaxww.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2helpyrun.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oxwerfym.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xkzywpks.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bpsjuoum.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ljnfvwyw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsmebyci.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xqoewgpk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2znqnvvdg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zgzhynjs.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2otlchxcu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2pglkovox.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ppdhjltr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrpkdzlc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2toiyprkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2styjbmjk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ceggnbmi.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yjlkglnx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xmzexfdz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mkskrdkk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyvbysqr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhnjtspv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wjciqapz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2lpklxwiu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zubmawji.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2sjdowupr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2dksjdkky.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2snslbbsb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2khchjknv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zjkxofls.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ljclqvdi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2yrdvnxaf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2apqmokav.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2apomzuhu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2neliysgp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zmwdqozf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2onduixek.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kjzyqlby.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnifwoxm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rbblalhg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2olezhddi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2naifowcw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2cnkauczj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2gtzqobsu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2yybjqzeu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2prjznluz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qatsorqh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hmunmcww.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2zbjtaqaf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ksuqxqhw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xopskvua.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kjgqznea.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2unfnihnr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2quakvwuz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ouyrkngl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bmbcalez.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hwobhagh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bqnsdmyl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2srgcfeck.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vcgjwlhq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2igiwjtxu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pxvshxis.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gfmxdjwj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gyardqag.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mmvbohzy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ekoacoro.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2iptexzff.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2gdbzhaiu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2orxvnvix.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ygqfxzeg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2sinlsgnm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2mcrxfohf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ypyllvtl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2japwgnwu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2fqwjqrxt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ohdyiusj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2awozjfpq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rsrmxisq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2kuogghcs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ksgvgebu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lypxxsmi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpihcewn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmsamqgb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wmixudwu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2betlaqrj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2etgbvzyq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xoshhjwe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ugtlryfm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2nfombcyh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cpqkmzqi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hwzhyxxv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tdwkleuc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gdxwkxvn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtmxfnad.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2udlrezrx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgnzmlhq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jvmvgkcc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ylzaeyxv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2guzftfjy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ujyurgbh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2jkynzmzu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qqvxcizy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jhmxffrn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uddhagdy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2lzcmndzd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jhvtncvz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pcanhmvn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fiwdyhxb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wbwgdmyo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rbloxcxa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2tguiungs.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wfqyxaqz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zjdymzwb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2askskgpx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ysqpgakk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vrmqtcoi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2teeqqfoe.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2luiwownt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dmusgusu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2eveztpng.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2tzujhjha.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2mjruvoka.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2grldfgoo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tsenizzz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2pvtzobdj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gqlwcuzt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vvuakvfu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2mrylgezo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2abvelhtu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nroejlic.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2rvqxxinv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ougfvdnh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2aitbyncl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wfzgcawd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2isduduzt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ryfaohdr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2miwzpoxk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqkzvmsl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2dcrpwofm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mxjljaar.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kwinwtaf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ioyrjpbd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qblakfft.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lnskejjr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rxddoaos.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgjocmkt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufehzajn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2klqafpvr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wqsveaca.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ijlwanbs.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fbnqbzci.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2gkrhpduj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jarfcuzx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2olhjsjqy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2lykgurcq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2cjukafsm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxvrxzkv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xqrzgnpd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dxidhvui.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2spgybyaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oncjqzxa.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vtqlypjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zlfqckxg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fxawftoa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2xiahoirn.html


<!-- 参考信息 -->