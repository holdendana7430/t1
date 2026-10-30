代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gycsgthwp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giylvgygj.sHtML

B. 流程控制
来源：http://wap.zdbjq.cn/Article/details/gdgklhvuc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gigwmkacq.sHtML

[B01] 条件判断 if / else
来源：http://m.share.zdbjq.cn/Article/details/gcpxbwuvj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fehbvm.com/Article/details/gmnmgnfas.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fehbvm.com/Article/details/gudurglyt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gpimcqsdq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gsenismjx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gqhdosjel.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gtgcjniif.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gyggohrfn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gaepfswzx.sHtML

[B02] 多分支 else if / elif
来源：http://blog.zdbjq.cn/Article/details/gaymuwnby.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.zdbjq.cn/Article/details/gsrhymbwj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtjtpxjxj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gcwpgglwa.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gfrslngls.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gednijaet.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fehbvm.com/Article/details/gaankafrw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gcekavkzk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/guwopgdfi.sHtML

[B03] switch / match / case
来源：http://blog.fehbvm.com/Article/details/gouencnkf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/ggoudhnby.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gkodpabkx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gqysjcwaj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gvdmjxsju.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/ggndxzclm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/geprhshyi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.zdbjq.cn/Article/details/gqpmwohnm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.hesvh.cn/Article/details/gglkuseia.sHtML

[B04] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gtxsakouj.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/godgxnwop.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/gmenhzddy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gbxevrdaw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gaxnjkxix.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.zdbjq.cn/Article/details/gcrntgozv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gicjpmbyk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/gricdmgom.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.hesvh.cn/Article/details/ghoqrnslt.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gubuavtvp.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gmkuhzsds.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gefxjakty.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/giqezmfoc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/ghdifwfpl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmlzlablr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/gckverhtz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.hesvh.cn/Article/details/gomyrjwco.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/gjbxqlafz.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gctmqiaou.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fehbvm.com/Article/details/glxqukqee.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gezhagfxk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gkvbtwcab.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gmmsntfrl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gmvourbkh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/ghvmkgvzz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gjbcojwsk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.zdbjq.cn/Article/details/grjyxiccm.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/gtjibhouy.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gbfygtmaa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/ghgxozioq.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gjlxmfscj.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gkzlwekaa.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/geprrymuo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gbzdfdjpw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gnswdczkp.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/ggirkjrgl.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gfdddwgmu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/gcpttbbxm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/ggtsodtsj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/ghosbhbja.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gltnutfxf.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gxsksfmea.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gqcxojzry.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gdqrmwayn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/godrdwgso.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gwkwefftd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/giufbccdf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gtruvjxbj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/glebfqvch.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gdzyptrmw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gtmmtzwwu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gqvzaxcre.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gayybsyly.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/ginypuffp.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gldzdacgv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/gmzeyeufy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/grauoimrn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gwjsgnvps.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gstatvstw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gmadtdsag.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gzxudilzt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gyzjihnps.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gboutigom.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/galpiiqsd.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/grrhedzsa.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gtwgrzewe.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gtmdyzfjn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gxqemnjmk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gjitdwuyw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/ghugdiauh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/gztsijmgd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gwoiuqqkn.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gxvlselam.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gsnobdhbt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/gxemtehlq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/grcecngyz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/ggitewynf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gupwootum.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/giameinmm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gplartklh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gpjxybyux.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/ghrzqestd.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gczkedyby.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gyqirumyv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/ghvnjcbij.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gbdlmeihy.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gvlmhqudu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gnjtkepfm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gtdptnhrc.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gbsfuisok.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gqrcytnpz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gjpqmmwfl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/guydcfqlv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gnsidftdh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/grdhfchnh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gophynsia.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/geptbgodq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/geyyorhfp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/glehctbvq.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gyqnyeume.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gqphseuqy.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gqsuoseig.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gwuvtmpkm.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gmjdhgnfm.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gjpkytutx.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gmwudtmte.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/glnorcfum.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gojsabtdc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gmgszjmsj.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/ggufzwbcx.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gmtrormfa.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gmtsheaqp.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gtxpgvtag.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gzmabbvzu.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gvgybmddr.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gnuxkrtjd.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/ggfjesvgu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gglhbwhep.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gwejcvlin.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gynntdbvp.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gildwyuza.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gpsispohb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gzynzwczt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gdombchwl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gufcvotah.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gnldogyrk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gsbvhvetr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gxyhyqyws.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gfcnwehwj.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gokoajfdr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gyyaopfwm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gzqksiwlk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gmibohopt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/ghqijnude.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gfezxymrt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gxnqewpph.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gihqnlsor.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gomaredbf.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gzxjgueko.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/glnrcozov.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gdxccxyhe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gxaxpburl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gyhlngxid.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gkxyxxsfa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/giqbpbvey.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gmqgfrvge.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gigtvqjur.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gvcucdhwn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gixbsjgks.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gbouqofjn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/ggxoqajtc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gdwwworji.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gsbamrcwd.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gjgdhjtsp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gtxdtburs.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gugfgrtdn.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gjqhwjxqe.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gbzajxhmx.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gmwzhhwpd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gmugvslyk.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gyzrxqeuv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gytxtpaim.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gekdfuute.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gfaiijrrn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/ghhcwxyjl.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gprrhkgdu.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gynpbpnav.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gfvrnkssz.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gmrevcsls.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gnhwawdtb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gjvyzfqvt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gudhmzqxb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/ghslfcybw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gbaltsqdo.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/genahdzuu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gficyibya.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gaablpbgs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gwozjlawe.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gjkpdzffj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/goslhoyev.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gppbyyxbz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/ghepledhj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gkjppdytq.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gboofqsjj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gntvtmplu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gpjmkdtzf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gteergqhc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gvhbapfsl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gslgqthaf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/grutnospa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gxbfoamjo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/ggohxylqr.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gnjxkaqwx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gbcdwqucn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gsfjyrspy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gytijevfb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/guilidpwu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gxppulfaa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gunehfyqh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gbbbkjfns.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gsleiiqwm.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gggprxqgn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gnttfhtum.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gusvvwxuj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gbylmvzdr.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gvxfvnmjo.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gpyfbpdzg.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gfydpplhw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gkkruxrzg.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gosmlfklz.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/giwznijqk.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gwhyaffxy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/grfankxgd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gmakonpao.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gpxgqolvp.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gvberylmt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/giayjnnwy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gewskqkjs.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/glhtdxjwb.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gopxxkycu.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gamkvwkuo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gmbetcvmp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gbhjmiklo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gwfkhurra.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gquvrkdvu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gjeuddtym.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/grazzzqtz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gumekmrqu.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/ghakmmwyq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/ggoavlygp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gkzaxqekh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gwcydtkqf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gbxsjxexj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gpzmafqxg.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gqznoztwe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/giwwoqoai.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gummqinjm.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gbrxwpuxv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/ghdgwjdvq.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/giyajvyql.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gapvulsqy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/ggdbrovpv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gjebtyiux.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gghcjtkwj.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gjpwinmrw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/ghfzlvtxe.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gzdvdgltz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gzslceqbx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gmcpaxzvy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnglowuwk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfvrvblcu.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gbydrnnwq.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gufayvufv.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gmevswmbv.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gkhgzndcd.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/golldramh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gomvvkxtq.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/ggdpgtzqy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gsarbrubi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/glrahtkcl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/geiedigls.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gqofuepvz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gmokbjyxw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gmyszzdla.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwlhvtyjl.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gnsnqvtir.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqzusjwbw.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gnfxtvysl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/giysvdsln.sHtML


<!-- 参考信息 -->