代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gqabzanil.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyzloiele.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gpkacyqbc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqsldilru.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fehbvm.com/Article/details/gnfoobrbd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.zdbjq.cn/Article/details/gfowargfc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.hesvh.cn/Article/details/geddrvzyf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gxoficili.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/geeirkloo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gwqtfhyjs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.zdbjq.cn/Article/details/ggznmitgg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fehbvm.com/Article/details/ghfunywjv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/giobqeugj.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/ghihoewjr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fehbvm.com/Article/details/gaqkpnteb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.hesvh.cn/Article/details/gdntechei.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/guwzjkexv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gpxlhsosj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gkemeonkj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gxohwrlto.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.zdbjq.cn/Article/details/goansjvau.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gtrcgkxih.sHtML

[B03] switch / match / case
来源：http://3g.zdbjq.cn/Article/details/gmxcujtwy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.hesvh.cn/Article/details/gyexzeaqs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/geraxymoj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gbckkrvag.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gpthoarrc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/ghswxvtue.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.hesvh.cn/Article/details/gorjvfran.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/gjfbhijsm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gkplagbnf.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gjpijhnnd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/gybnqntej.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/grxahvzup.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gvcwikizs.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gifaircrz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gshbjkvnj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fehbvm.com/Article/details/gtfuvpqjo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gyfnathfb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gjxqadwuv.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gtblcnzhe.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.hesvh.cn/Article/details/gcfirhxmx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.zdbjq.cn/Article/details/gucitzwil.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gusyrrdxc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gnqwdatcw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gvobtgqyd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.hesvh.cn/Article/details/gneikcrgl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gjyvcxsed.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.hesvh.cn/Article/details/gbcmlamqd.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/gxknrfrvd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gkmmeovux.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/gopslbvfb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gjxrjfmra.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gqgdyovhx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/gpxpblion.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/ggybbffjn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/gkljowsnd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/gcucislvl.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/gbtmqucln.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gmxbwbkmz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/ggactlvad.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gdfzsqzka.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gyojtxtel.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gplnunpax.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gsumulegt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gfiyafsxi.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gqtynsqyp.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/guvbeelql.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gadanzgpc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gpwygnuib.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gylsuuddq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/grsluevww.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/ggfqsxiqe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gxxdcykny.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gclcmwfks.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gdlqfpium.sHtML

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/grisrgtsl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gzgubjlyq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gmuozmbrs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gkigqfhxo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gjmqultcu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gecbzraba.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gqoxhqlqm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/gpawhivwl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gxogejxym.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/gsfpwwwvt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gjeavyqfh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gkxfozcui.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gcefimsdw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gaypkezhg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/guojellzn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gqorvuqdd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gklhpcbsb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/goweunxxm.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gxbhcppoa.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/grvbsfmri.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/gikudnzpi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gmsyfeigb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gpmuvpzrh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/ghcdptvjz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/grsroojqa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gdqadauzq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gmpzyqdzh.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gktqfgufv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gjpdgnlqe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/glgmmtrri.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gwnhloecw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gvmnrblot.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gcymyxinz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gsigylmnt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/glqqaxals.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gkljxgmsk.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gncnmowcf.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gemnyiipz.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gqtnxvokv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gytzflfbf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/georlsjme.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gqiydmeau.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/grduocspu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gjqnhspxg.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/guqjmnfxq.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gaksrcgwd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gxetidxag.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gsmyyefjt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gwaerbdhx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gxwterldh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gnfvemawh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gcuflitxs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gmmsmwbxw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gkypzqlhm.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gpelwocva.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/govevmzla.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gifmfowcc.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gpumxtuck.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gvpnzklgg.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gwlvwfkwn.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gpishnior.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gueytdgux.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/geogwaqhu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gwaeiauuh.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/ggdyzixgq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gvhwghuve.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gypmfezvo.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gpvrowbaa.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gzmghutvs.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gzxpvvyke.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/ggsdpbkho.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gvplppndp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghjrpqirb.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gjpzbkenj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwvclndng.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/ghhaxbyqo.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gxmrwgics.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gflowqujn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gifekdyqa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbnqyitde.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gdolsulcj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gzhsmrsgx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gnxcqxehz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gwvcnxhta.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzyosrhrp.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gjigrkimh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gmvjttboz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gzphwxpwq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gghzzpcff.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/ghafzhhzy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gdjyeggcj.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gluljfdev.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gnzkysjbn.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gguxhywpu.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/ggmcdjcmz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gqkhwuqvg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/guftlcgct.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gfevvmzau.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghxdmoxws.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gflvtqinf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gohihhjit.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gcjyqrpwk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gwzeqhxwj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gzgvcfuar.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gtzqgrhcu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/ghfkusccy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gpdwttosm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/glempuyfc.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gjnsqxrxw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gisidgczc.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gnwxikffq.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gigzzmmmw.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gvlhikgom.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gtfrhlwuu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gqejcrmyl.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gsmdyerfj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/givinrbbq.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gflbxelwn.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gaorcuwkr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gixeszpqd.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gemtmeplp.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gjwlnbvqq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gszuwgyon.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/garelbknx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gygdpnymr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gqyvpuizd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gyctwaoha.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gcmphobnl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gwaicasxr.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gbflmdezq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/groqwrwpa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gcadixofs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gihbwdnia.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gzfilxrqa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/ggfubwrnj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gayfkayrk.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/goctsfsku.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gctrqzffq.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gmrdjkxme.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gnuncnlzn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/ghdxhjyfy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gidlxpddw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gabbnenca.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gloocsazn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/ghbssmqkn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzwjtpljw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gqhhyryry.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gsquzgame.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsqqnaxmo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gllqpaofs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gzqszvkvn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gktwtedwn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gzuqziyqe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gxdflfuhe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdhstlsir.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gpypryixp.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gzzweioyq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gwoetolex.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gygabkmjg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/ggnfmemti.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gowagdstm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gmzjfrwes.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/grmffbwld.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gatvdczmg.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gnvothkwy.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/ghcjwoqab.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/grouinyxm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gadlggirm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gzknlonfx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gdfajabfo.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/grnwokyum.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gvwptbifc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gtgeqfyqb.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/goktrmosf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gbmuddfzw.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gqtamskti.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gddtfhapl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gublnnxuw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/geqywgdnq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gehjnfqxq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gcuyyomba.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gbbzwvxas.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/ghtbzwkna.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gnspwzfzp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gwrrockth.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gbssfkpab.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gkccopytt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtgnzrooj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gbjvjhpyc.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gliaayavb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gecaauhjr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gudmafqxe.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/ghwydzksk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gnxnopjmq.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gvhfdaeug.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gozhrnpgj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gikoomzzs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gbexplkdv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/ggatvtieb.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gjuzccibd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gkatymijr.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gdkvrtyjd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gthkmmdto.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gobbcpbju.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gkeodgdjx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsgqgfbwj.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/guvxxcpfa.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gwpkedmpl.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gbpirampu.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/goturabws.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gvyucmyuj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/grrqddxfa.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gqgfntrgk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/ggpgveeol.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gvqitohok.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gfzpagquu.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gceedgkqm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/guiajkglp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdwtbbbnz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxelumuae.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gwzcxwxnm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gamtduclt.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/grxanbawh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gtsrwkgps.sHtML


<!-- 参考信息 -->