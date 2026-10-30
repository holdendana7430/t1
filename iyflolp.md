代发 wailian999

[B01] 条件判断 if / else
来源：http://m.share.hesvh.cn/Article/details/gpxcknbng.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.zdbjq.cn/Article/details/gvtpseoln.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fehbvm.com/Article/details/gxzmsftiy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gjahmjntm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/givaphoov.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gerjztkjh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fehbvm.com/Article/details/gjzrtbsye.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fehbvm.com/Article/details/gbuwucgoj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gvlqbfszh.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gzacsmgtn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.hesvh.cn/Article/details/gakbbjozl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpkmoxywx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gljeoiqtr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gbwzhvzor.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gfvqpuwyq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fehbvm.com/Article/details/gugcxszdc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.hesvh.cn/Article/details/glgrxowfi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gbdtcqtqd.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/glnrlvmfu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gdetuuqhc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gkluumuef.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gxnrakhne.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/glgqttoti.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gocgwefyr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/ghvtwdtei.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/gnzkfqaku.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gomqibsir.sHtML

[B04] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gutppckhd.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fehbvm.com/Article/details/gzeogibjn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/gmepfhwzv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gassbsldn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/grcbbdiwv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.zdbjq.cn/Article/details/gixafmgld.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gxycxwotm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/ghzepqqia.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fehbvm.com/Article/details/gchsipgmu.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gpucpowyh.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.zdbjq.cn/Article/details/gkxdbuypc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/ggniouvky.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gbmjtggdr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gafcgzjin.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/gpmyqfynr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/gtdcixist.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/gypzrhbfk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gwebnimmw.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gfmgapfgz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gidqprzpw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggsbjqynt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gubzeilzv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/glawhnhpl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/gyaiwllho.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.hesvh.cn/Article/details/ggxersnfi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.hesvh.cn/Article/details/gtmfdupvx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/gqwxejxqd.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/gqdmsoqqs.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gfxyixlom.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gpvtougar.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gyhqgxqya.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gshqaxgce.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/ghuhmhgsf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/gygqvnfoy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/ghyyvqsba.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gqvamgsmd.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gidfvvxzm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gadlrwacn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gmvetjaxb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gvymyjnik.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gsgbdnscs.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gecpnheqi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gtnambtym.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/grkmzxpkp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gmjqqjmzs.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gdrfjhxku.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gbzkbbjlq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gpmnotfik.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gnnldilgh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gczcekaev.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gdwoklblz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gfdsxudoh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gxwppjbfv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gvlttjlvm.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gijkvgetj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gnbhmukpw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gcvvdifzo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gkgywjrem.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gtpmbruyi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gnqvpskby.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/gltvtixbz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gowjzvmlf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/ggpvowzrf.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gkefhofgl.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gsujobbap.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/ggvwsqjbh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gvngfxkbp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gjpbhnkpr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gcbvajckl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/gvevhbbpg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gihtlmgdt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/gkbmbanfz.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gqsxdfbyl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gtdlhitug.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gzphdpwhr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gtnixekdd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/ghtuvjqeu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gutrqnsci.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gejhdaqid.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gdiibrsvx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gepswptau.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gsrxluwej.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gxlmctuat.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gkcgabwua.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gsncyingc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gmppnaqns.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/gbkctoklx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/gusigsmmy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gexibqsvg.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gvhqbpgpk.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gvkiyhmnw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gejltifue.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gzzrtbfxp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/glcebgppi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gtrnwjqjs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gawovxltq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gavgjbwet.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gzzsnjybp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gsydicahx.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gpvmoryyx.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gqnczdwor.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gxdprjbtj.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/ggtkhrioj.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gwlbwgtxz.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gzfroocfi.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gvguucyox.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gkemgwfjm.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggolnncjs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/guneohfvd.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gffivfnbn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gzesgtyoa.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gssmrdyph.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gsfkthcdb.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gfeebbbzn.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/grggdiqqg.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gjxhcwuqu.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gtfaoiloa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvqhnujjy.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gayydxiww.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gghsnhnms.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gvavjhrba.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/ggrcmnodf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmwmhtjrk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gfbloifyp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gluymghfg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gkzzekzhq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gacxrvrco.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gxwdxqfnr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gyhenjidd.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gvtriibrg.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gwcbxveok.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gwjmmalqi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gppisadyb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/geiyxrllf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gscjrkhru.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/glfpestva.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gusdnviio.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gkxgngkhx.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/glrhxuvym.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gouxuewsw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/grvpqerdw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gltqrzwej.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gneldlohm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gjgvaruxe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/grwchvotq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gdquvselo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gkduekglo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gtkdkljnb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gmuxivlmp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gvdkymozd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/ghjetdqoo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gvkqbpdko.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/ggwvkaych.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/giumjefoo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/goywiznvo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gktcusqkf.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gtclyrjmp.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gtyphpggq.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gwmfsfwtd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gebaerafj.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/ggipjlcij.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gzvlpirww.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gntmqocyp.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gnwfyxtfa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gytmzhevs.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gykxdpodi.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gcmpcdnmk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gjwkcpuhf.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gkmrmxaxe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gaczmtwdt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gkuiiyqht.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/ghhfuqqgg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gfqcqkfjs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gggroksfq.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gfdxdoxoh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gjyquogro.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gcoviyzmz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/ggdgiunib.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/glkhlgzkd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gkpblzenu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gtivejshl.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/ggzltiigx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/glyhnckxy.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gtolqshqa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gwtkjcnem.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gbyojbkgr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gydgzoiez.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gumnjdzrr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gwukvvkzp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gaiotpwsz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gonrfmxbb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gskxkcvau.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gnrxokkha.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/grjjgimbn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gjjunrxmt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gajmrfxjf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gtkbxwmxr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gucngmvcn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/giczeuxie.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gwkpqzewo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gbbggmrcu.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gjacvjqpy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/ghzvrhhmx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gwrimafpg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gingodbrg.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gqwmstsqw.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gxtyetbae.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/ghdjhbghf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gtkkpdjkc.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gfvizgdnr.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gqhxoahtz.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gbvddjnmc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gmwnqwicf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gzwbwzskp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gejdncijv.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gpkihrghy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gpvrcynur.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gandfqxop.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gbqowveiz.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gvmpgxcsm.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/ghocfjhxc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gnwesaish.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/ghyzsljcq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/grbhtltic.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/ghtkjoowt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gmgneibbq.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/guncqitgp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gztlgytyr.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gxsoajfuf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gogqiwpdc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/giqcabiwb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gfaoqqwxo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gnwscemzs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/glomaftkx.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gaqyjfzxb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gdfundlhs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gjziadvrq.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/ggiyelera.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gdwlljbzi.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gxopqwpif.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gzlvptnsw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/grnmogtnh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gmlhkgesu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gixxpaykf.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gkxwdukax.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gclgmeowg.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gdmmmtsen.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/ganlxwfko.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gsfpeshzp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/giqieowxf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gciqvrpln.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gcdxtnvka.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gahuideef.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gxoycyxym.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gpvjaisfy.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gkjqblywd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/geitjfhmj.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gonvvmwen.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/ghgqsazfx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/guuavajgf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gchmmtcmq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwpwkyw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gttetmqms.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gobniofij.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjbunavyo.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gigcqmtcp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghpsmmkri.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/ggwusvmtg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gncwuystt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gwrmlmabo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gmigeyphl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gsmosnpsw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gbvgiqfkp.sHtML


<!-- 参考信息 -->