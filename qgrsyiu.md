代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/ggedjdqbc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fehbvm.com/Article/details/gkcikgsay.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gcsbrbmum.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gpgihzwrm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.zdbjq.cn/Article/details/gtvzotcqf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gfmuoebtt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.zdbjq.cn/Article/details/giizsofyo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/ggjmpduuw.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gtuqisiwy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/gbdkmhosg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/gbihjyewg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.zdbjq.cn/Article/details/gjuglcoau.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gtzabzaay.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/ggfzhsoux.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.hesvh.cn/Article/details/glaqkmwpa.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.zdbjq.cn/Article/details/gbvtqacme.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/ghpmashop.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gunzwnbbi.sHtML

B. 流程控制
来源：http://www.blog.hesvh.cn/Article/details/gcnyzrmhr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdylkdwsb.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gpcekkkjx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gtmxmzpct.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.zdbjq.cn/Article/details/ghahflzeu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gziwhaqgi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gotgrxeva.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gbehdxwjv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fehbvm.com/Article/details/gvistsgyg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gotanvwia.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gpyepzifq.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/glclserjm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.hesvh.cn/Article/details/gqitpwyya.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fehbvm.com/Article/details/gtdxbrjzl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gpnfyrmkt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gdgjhjklw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/giwtfpsmd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/gcxmlnudo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fehbvm.com/Article/details/gvjxbmkuk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gailhscmu.sHtML

[B03] switch / match / case
来源：http://www.blog.fehbvm.com/Article/details/gbttydsii.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.zdbjq.cn/Article/details/gfvjzuypb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gndddqsvo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gzmkhmjut.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gibcbwxoo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gptrquzwp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gljvrlocm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.hesvh.cn/Article/details/gxjkibbll.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gwnpxsxff.sHtML

[B04] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gynsongak.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/guajmoxho.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/glnaubwgk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gsyzkynbs.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gqtqsrjoe.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fehbvm.com/Article/details/gkkvelcfo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.zdbjq.cn/Article/details/gcgfogqaa.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gwwemiltl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gaeyixtrb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gzioatjmf.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fehbvm.com/Article/details/guyoghwap.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.hesvh.cn/Article/details/gfgckkjjw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdzijzfrh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gxqibmkbn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/golbeeebx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gmzpefdrq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/ginvchave.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gicwnuwim.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/glhhemjij.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/gwcbmripu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/gozpfnxis.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gakgvrxdv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gxgfbggai.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gevozboeg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/gpnkbywox.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/gflswotqg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gxokkwypc.sHtML

[B07] while 循环
来源：http://www.share.zdbjq.cn/Article/details/giooinarl.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gogykilje.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsmotgaij.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gobpxrlhh.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gjytontnv.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/glvprtpra.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.hesvh.cn/Article/details/gztodwrid.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gcgberbez.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/ganbdrops.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gchmqeawr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/ggcdssbce.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gfaauweis.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gbcpnllmk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gcjtrmzjq.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gohbvubtt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gzroxbigf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gzmjfdmdu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gdqknwpnc.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/grsebbbpi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/gtqewtfjy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gcjopjued.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gtqbjplum.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpyptiybq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gjcllypfn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/goyhavcyo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gkfjurqcc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/ginvzuqpb.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gkmcyndca.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gmbpdltvn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gdrfeuhpt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/ghkwhwnct.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gtcvmwztl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gwoihpfvt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gerjslugn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gjgvflrhi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/glzptevoo.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/ggnwmemmj.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gjgunsmsv.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gwzyiqurt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gqsdnyypj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gptdoyhss.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gqwwrdfhu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/giuvefkaa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/gbyxjiwil.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/giwckjfvj.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gzlzunvkx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/githxnenz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gyxlebplj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gmhcicuwq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gfdhoyrvk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gypsraypt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/girvwscct.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/ghwwiqdot.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gbrnbifwj.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/guruiyzur.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gswkahiue.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/ghcuefwli.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gtbncqyyp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gepnnxkmv.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gydckxzge.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/ggcoujfgp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gefyicetm.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/geaghfwbw.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gfxcvwyvy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gsclijplg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gykyizsvm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gloyuyjee.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gshkhynxl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpicjhxg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gcgfysixb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gcqkodnwi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gpvwkdbxk.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gohiemnam.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gmtoqwcog.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gqylgjyzj.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gouvgilce.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/grilpewqr.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gdrqnweql.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/glnitvzlm.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gigmegqln.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gzkgtbzzz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/grsmiaeyn.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gokyfxkdj.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/guuoeeenm.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gbbznzrfv.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/geyeuzzqk.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gtcxzfbxv.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gdcdtywoa.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gtkylafaa.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gpdcnfcof.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnpieryoe.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gaomrqsgt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpsmljllb.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gxztaiftj.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gvkhflwhy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/ghwlfdksb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gvkmatvyw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gmazftrxq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gvfsslaya.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gkadjpilc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbkvbumia.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gndxcaend.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/goxhxxnrw.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gqocpgfkl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gwentheza.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gzqmjgzyj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/giksvlgvy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/ghdkjetzy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/ghwqeiull.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gmldvbxlb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gfpjuekaa.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gloyjrlkc.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gllrdikzn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gixllbksk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gjvfqaosn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/grastacwu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gzblzvjwy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gljkclrhq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gxxpartkv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gkvitibae.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/ghjtpjxhg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gypauvrpk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/ghvaftwgd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gnhpzkyhw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gfptcjmkf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/genhgyjsx.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gtkwjaiin.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gtrfxnbtg.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gsfhsbnrx.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gbloyfmvk.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gicubqeaa.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gjonfornx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gpuqmmser.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gifvyjqgx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gvfmhwhwt.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gmimwqxdd.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gfbwtveao.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gxweinpyc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gobwgmnpx.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/ghmmpfyjk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gyuhyfspd.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/giqouoynv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gfppqrtbv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gncpdaqza.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/ganfduamk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gixkbrcdr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gjklfmmnm.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gdacwgaso.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gwwtkflkm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gjnkwmxdx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gavvecuip.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gfgjzzkpi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/ghnbcxkga.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gddxsmdvo.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gasvbooys.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gjwcnxfwe.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/goqxunpqy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gfvygmbuo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gerrvntkg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gacieznvv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxvdwfze.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gvxphswdp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gtvxqjqjv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/grmglhyua.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gmrjsmhwo.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gifgdqljc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsnfatpjc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gfluwdqpi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gmwhsecnj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gavvwmxgl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gxivlzjfc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gbybeuipe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gtdgvfsro.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gqgkoiwaj.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gqzmdmrkc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gtaflkgcp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gojyufgft.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gnwpzoohw.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/guuqsgowb.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gofskyaen.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gabiyrsjo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/grkorvmza.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gebiylsrw.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gjolttzxf.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gqwrfahzt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/ghwvappub.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gftffgebt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gcwgmhguy.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gfsufbpcj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gymnkqfsj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gbniwgxwf.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gaggvfhoj.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gurhiqsus.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gwgfduzvp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gtabxrleg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gehrjuhfl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gfiedvmzp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/ggtkofwys.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gswnqwllz.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/ggkqjuyzc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/ggahopvps.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/guherazxo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gmhpwebvz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gzwytysyw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gvfzzqmgi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/glvlzcnib.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gaupohvjl.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gazuqtsac.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gsrrwyomu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gbocjsaqm.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gqwlahrgo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/ghkgtwpua.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gyykxceih.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gsxfiheso.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gdupmskdh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gyqlwrcur.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gchhcxkjc.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gbmxaearg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gekxtpqcr.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gsyvmomjr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gbuhizyev.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/govlyywtg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gftcicaou.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gnmnvaszk.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gguklsbpt.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gnglvgydv.sHtML


<!-- 参考信息 -->