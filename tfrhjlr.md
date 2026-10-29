代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://m.share.fehbvm.com/Article/details/gdwisulms.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/gcilhypvt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.hesvh.cn/Article/details/gbpleinmh.sHtML

[A25] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gktpuwvff.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.hesvh.cn/Article/details/gjxhbprao.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/gbswyogrf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/gjnsxijvg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gxtswrrch.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.hesvh.cn/Article/details/gyyvwflwz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gdsgvrlsz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.hesvh.cn/Article/details/gwggvkdva.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gyrycxhmp.sHtML

[A26] 类型转换总览
来源：http://3g.fehbvm.com/Article/details/gtvkgzdlw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.hesvh.cn/Article/details/guvvnmixm.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/gcfttnknb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.zdbjq.cn/Article/details/gcgmxophm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fehbvm.com/Article/details/grcerafop.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gtbkeuwao.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.hesvh.cn/Article/details/gebfpappx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.hesvh.cn/Article/details/giiuwtben.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gclcjpbbs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmbuoajce.sHtML

B. 流程控制
来源：http://baike.zdbjq.cn/Article/details/godqhmoin.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grdkcpmnf.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/gnwrrzdyl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/gzpggfjbm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/gyyjiipmc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/ggznyvzdt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gweqieeur.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gjokpndau.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/gqjmfccsq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.hesvh.cn/Article/details/gksjipeqe.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gfvipusmi.sHtML

[B02] 多分支 else if / elif
来源：http://3g.zdbjq.cn/Article/details/gaznhcrzf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fehbvm.com/Article/details/gdmtfyumj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.hesvh.cn/Article/details/gnwndggkb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/ggudewsqu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gixwoabrj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gfllovhez.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fehbvm.com/Article/details/gvfzqwlaa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.hesvh.cn/Article/details/gukedrngn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gfyyyzmdk.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gvhkucurp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/gxgfgbufs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gpwzsncst.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gmriuwaci.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gctourmzi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/guzzctqvt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/guerwzahw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gjyftgogl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gkvomhypu.sHtML

[B04] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gyrdajqmq.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.zdbjq.cn/Article/details/ggtqqvcyr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/gyoxgnlqg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gvwpwgwtb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gbirpsulv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/gdxvzyxdt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.zdbjq.cn/Article/details/gqytajhxs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/gatrisfsk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gnirjofak.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gmrbfzcqa.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fehbvm.com/Article/details/gphjugdxx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gtgosabug.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gvisyvdbu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gggaczwec.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gdswabwcj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/geprupeqg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fehbvm.com/Article/details/gqhvazvew.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gxaqfatkx.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/gvcmoirju.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/gebjwawwm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/gbsypchkl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gmfckylqg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gxwlojdgq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.zdbjq.cn/Article/details/gsqvibzhs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gqwxpdjic.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gugkrpjgs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gepevdhbp.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gcymfuaee.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gtkkbmgwx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/gbsneshoq.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gapxnrclt.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/guygbfkwh.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gyfeneqyu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gbptgczjx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/garbfptxi.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gikoedsos.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gunnxtwbv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gsfqgngoe.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/ggkmwxqlm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/grghxxmug.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gtprzcqhj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gbwnxpwlq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gnzwtraaz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gfrlscdok.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gtdrzkybx.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gnatcscrb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gpamjhlfe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gddtsfjbn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gqqqesivb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gkscuhjoe.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gijdcoqfw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gvqgsgmob.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gsitdrrum.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gcshgggns.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gziqtjdsk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gkixnczcd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gqqtzaxwp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gxhmwfbov.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/ggtezbxwc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gskukyzik.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gmtqeepsb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gembqpzcr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gwnrgtkhb.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gayemvzte.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gfmuacrhv.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gslitycxp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/ghderzzms.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ggprjckdb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/ghddnkscj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gwvgppjny.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/gpaxsxltf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gxmldsizu.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/ghyseaabl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/glhzogmbq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/ggwckgfhj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gttssetox.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gmdijjrbv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/giojeygjn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gecawqynr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gzofqpdva.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/gzcqapaap.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gkxzyaeqi.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gakjdwwdn.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gpgkdtcse.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gpkxlwpyg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gigrlibuc.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gtgaiyqge.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/grnguetnu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gfpkgilnk.sHtML

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/gfkiceqvg.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gmtxxvejg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/grusrrpwj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gqplzbuvj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gqzknhyrf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gpubzojsg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gogdehydw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gxgtswvkk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/guhfkhysy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/genpehenf.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gsizdbddw.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/goodcfomm.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/ggpsbmevv.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gfygwrffw.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gcicxncey.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gkvrxtlhk.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gereunjii.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqzrfarhv.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gsheslvoa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gevpmlwlr.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gfdbzeykz.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gokaoirks.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gwvrrgbbf.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gwlbvwgzu.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gjcvhwliy.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/grylkqdob.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/grevicwhc.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gbtsmhzvd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gncosrlgb.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gtvmrmeuw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcfdnvzcb.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/guckepsqx.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gcxmglcld.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gsrgoawro.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gponxdjcu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gblunumov.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjexnrhk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gqrftaxlj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gzojgavyl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gwhkiyivj.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gagxrifty.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gvhikjyzl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gkmxfwghq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggedclilh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ggzawiibx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gjmveifmu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gwcffbsmt.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gkomktfnm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/geasakuxt.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/ghospjpyz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gkiqkjoir.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gllkikiig.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gyxaqfsnd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gyqragefl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gyrpglqrv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gdvwogfyq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gfbjknegf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/ggafqxxuz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gnfbduvkj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gxlhxwykt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gnijewcxh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gxxtrahvt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gmhmqjzsw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gkyxwxrfa.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gecsbzmpd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfqmbnftl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gicfymyoe.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gjolbihrs.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gvmauumtk.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gshyursfy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gfsjijddt.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gwihwyeol.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gyspgktbx.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gjgmpfcxd.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gkamyyvec.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/guxjeyzjf.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gehbchhtg.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gncezzyry.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gvwntuptk.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gcojoosnh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gpndespzx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gqougyrhh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gjjkkdbrx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gxzartmhd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gviusiivj.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gidlvgoey.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gkfcpiusd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/ggqevohmc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gtsfuvnok.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gjhuvejyp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gtnbsjqdu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gzdulxpnb.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gpyskxhfm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gcwfqbmto.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gfjqtxrvf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gtzvmhzuh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gvffnxfed.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/grqybbgdw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gyqbbmybd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gjwrltdas.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gryypolgk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gnkjncjhi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gpisqhudh.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gbghnkzsf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/geuiwatiy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gcjgyfxxw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gciytlivm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gqxyhmcrx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/grlxwajgs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gjvwlhrhd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/guxomotlk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gqtvljnva.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gmqnwgbtr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gebktouvt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gzqktsmwa.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gcxwqwjxj.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gsprwovjn.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/grnnkztnb.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gfukfwzch.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gftgpifid.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/godlqifjh.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gwadanbku.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/ghjwfnuju.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/glftxhlai.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/ghalcghxp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gfmrgijti.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gcvqxmckk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gvwnsbwtg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gyqgcwkup.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gkhlzjujn.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gdrtqfrfc.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gzizybtys.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gtryzemds.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gqrwlbiym.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gboicmavg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gmczsrief.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gicqijdsk.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gpyitdkco.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gdpifgtua.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gviuetuwe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gydxirtzd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gwdolxjth.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/ggauaqaav.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gcqdpmunf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gobswnkrq.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gwcavchtl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gopuxvrit.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gjcnxajuw.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gwzqoqhfi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gqezwmtfh.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gjenqwbfb.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gcsprofps.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/grmgdrngn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gmqutezep.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gtdlbltie.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gqwkxhumr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gtmkjdywk.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gnbcdxbjf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gdlvzujaq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/ghunclejj.sHtML


<!-- 参考信息 -->