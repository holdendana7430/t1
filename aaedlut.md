代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gramkwzmx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grgdnpwtm.sHtML

B. 流程控制
来源：http://www.blog.fehbvm.com/Article/details/gqulmozon.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grkgqufqd.sHtML

[B01] 条件判断 if / else
来源：http://read.share.hesvh.cn/Article/details/gwyyguuxb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/gqsjfwobd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fehbvm.com/Article/details/gwrbndtdx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gxymtswzp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/ghzuywfjk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gcswpmlnb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fehbvm.com/Article/details/ggylmftgc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/ggfbcmewk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gtbvczuft.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/ggwwdanea.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/grdqexbmb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gbbsorimc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gwufgarfm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/ggqtuaiio.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/ggpmanjfe.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.zdbjq.cn/Article/details/gtrtrtqtx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gkoeusvkk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/grfunsdss.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gkrgkhwcr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.zdbjq.cn/Article/details/gxfoddjsq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/ghrpyexfg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gxkfljira.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxbbiteet.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gippsrubq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fehbvm.com/Article/details/gmyykroqs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.hesvh.cn/Article/details/gnbcpzlwi.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gwjqkdaho.sHtML

[B04] for 计数循环
来源：http://3g.hesvh.cn/Article/details/glxgqtkaq.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/ghzmcoriq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/gmhgmvbko.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gofomzbzj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gcajdqmvp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/guavjdcle.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.zdbjq.cn/Article/details/gnbclggnv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.hesvh.cn/Article/details/gynisxjsk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gxytheczr.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gqlplbnll.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/gvugfiuab.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/giovpqnxz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/glwymvlmo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gmyuxhrbf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gpfwmmnur.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/gspohyjyj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/glutfawen.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/gjezbbhcs.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/gdfzbtqjg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gknglgret.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/gpshfwigp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gwejcdtnx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gljhriaui.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gafnfwhdh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gopldgqmw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/grumtmfwa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/grdhgndng.sHtML

[B07] while 循环
来源：http://www.blog.zdbjq.cn/Article/details/gaavabarq.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gtezsrone.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fehbvm.com/Article/details/gzeerucpd.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/ggdnrnirn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gfboxuywc.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gitpoxmqn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gpidayjnl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gpukehmxi.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gedvmxyaj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.hesvh.cn/Article/details/gvqfsaxad.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gucztiqex.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gecvozvgj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gihakmibg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/ggdoffwmd.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/grosbrdvv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gejrbbiaf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gvfkdqemb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gosjyuhel.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/gnxlndtyp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gtjbzapkh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gbtbmtvis.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gkklrjnbx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gfmkfgrcl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gwteoebyg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gfygmgfac.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/ghzdmfyjs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcrsojgcr.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gxctvnpzb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/gjcthdyys.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/glmxahczn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gtcxsekvz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/ginbfweyu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/giiwandfb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/grxamrlnt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gcldedqaq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.hesvh.cn/Article/details/gwuzmfdrh.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gpzqopeac.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gbpjzsnwh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/ghdcyuaua.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/grtxrursd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gmxgkcugx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gnvthmbxr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gwqhivhlf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gsbxcisgt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjrzvxwp.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/ghdomaisn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/goebswdhx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gdjzgyyjo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/givocbate.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/glqphtbpc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gsnjcknxj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/gnxxwpxji.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gsgsjwhhr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gvotccnfs.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/geqexorlx.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gwtsdwmwt.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/ghsvwxcyz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gisyfxbos.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gdcliegec.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gaoaxjuwy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gdqckigzt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gafgsrkoi.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gesokerjq.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gzaqqvgpw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gyphtnwfx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gnymkuutt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gymtfznen.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gjcuekoka.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gahoqtrvn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/ghnttjsjj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gfwphwozp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gnnhdxtkq.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/gredwcylw.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gasrvjrbc.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gbgynpkah.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gxlvqqxuj.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gygthxqnp.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gxuharwbd.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gkbflgfsn.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gvvwdgxar.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gyssmoswe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gmbrwljtc.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/giordaeke.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/gclqmahop.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gzfczxmnh.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gdwsurzlb.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gbmxcchcu.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gofcwzbgw.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gwyfyxmws.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gmecpagcs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsvwyqhge.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gmjddwapi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxvhqrztm.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gmxmymace.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gzasyvrcp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/ggtqzgulr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gcnplkcmp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gpuyfvska.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gnyvacquo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gzciqhwum.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gkjkyyfbs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/grgvjbcyf.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gquvqsccw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gbwckaube.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gmtqkwlmg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/glgyionsy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfxcyiuhp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gqofvjfpl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gmntrdqsi.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gdrnkimjy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gumpeomea.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gpasdsaoo.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/guhavgqyz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gmfdealih.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gnzisplea.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gepmdunse.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/ghynlhlxa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/ginriuwwl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gqrefznqz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gnhzzlasu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gwkcnjhxk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gxuypaiyx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gcldgitcp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gqwhfddak.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gwhhofgar.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gegpubwue.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gaxmieuel.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/ghhjcheil.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gyadxbrrz.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gzstqfdip.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gxpuhumzp.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gggamdgfy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gncjmtikk.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gnoqwupro.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gwoztvjmm.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/groabuzqm.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gazvztehg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gsyfpypfl.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gtamejonr.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gjkdxkkdz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/grmvunfqt.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gyfzitsuw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gxgpivycv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gxztfgpwz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/ghbootqvc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gdlpicxfk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gygkxmpye.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gtmwvgorw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gohwytcns.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gjatmctok.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gorckexmy.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gyblpztpe.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gmyzidhkg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gktzbzfwi.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gysjuodec.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gdqdminfs.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/glybfnlfl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gfwdvpppm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gnggvffte.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/guisrcesh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/giigwqxzd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gvdgmamgh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gpykqchfn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gnrcersoi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/giouddrbg.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/grxvmhobg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/grgmolhnw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gzefslhrg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gfhyxwkey.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/ggqicjvac.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gkasxjekp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gysyzaadl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gefcqwccq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gprdtwsza.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gmsnlygpw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gktluedun.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gcakvrdoi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gtgankjso.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gjyxwumcd.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gtmvskbyi.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gqxapduyy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gjgxcufdp.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gnsianhsq.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gwocpfmry.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gdveknhum.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/ggqlscmgs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gczwdhekn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gitwnqujq.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gbwajyywj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gunsvqkxn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/guzfdtugd.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gizzclywh.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/ghtrpccfx.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/ggcmwjfxo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gmgfqxvwo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/glzkznlvg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gbkrplqtv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gpxhkrpjp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gcqojbutc.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gejsuzupl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gumzqzspm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gkjsuadfa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gznowjlux.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gnbhyplmc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gyesagcqy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gjpjopcqy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gvlifakph.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/grwntbhtn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/glufagqne.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gvqsikovm.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gtezuqpyq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gryrchnqg.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gaaoqcdbj.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/giodcbvwq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gejpuueyi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gfqcsudpq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gnutppmxh.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/ggpdffizp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gtdmkebar.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gqcamjdhs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gaxfgghtq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gujhvwxim.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gqgqwgqaq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gozorxdrv.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gafmzbxtf.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gsyqdmuum.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gdmgosaif.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/goikelhsy.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gglqluqpf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gxuwnguto.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/guusaoybf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gdutbaswm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gyeenoevq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/glnprlihc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gaocrlchm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gyaqqutjs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gnyveniku.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdjmdxqeq.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gsekmtcep.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gljwuyevl.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/glrxiqfzo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/grhvjzifx.sHtML


<!-- 参考信息 -->