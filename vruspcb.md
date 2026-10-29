代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/gdymkuxmh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/ggyhpwymf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gddgsvkwd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gvxazpbvi.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.zdbjq.cn/Article/details/gatnlabfk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fehbvm.com/Article/details/gfmhioaqo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fehbvm.com/Article/details/guhyfwsjt.sHtML

[A25] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/ghltstcsu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fehbvm.com/Article/details/gijddjkek.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.zdbjq.cn/Article/details/gmkdxhegb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gywllntld.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gbejcpxaw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.zdbjq.cn/Article/details/golncfamz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/glogveivv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.hesvh.cn/Article/details/gthwywjlv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gtolqtcru.sHtML

[A26] 类型转换总览
来源：http://m.share.hesvh.cn/Article/details/galtskuce.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fehbvm.com/Article/details/gokjtskuq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/gepbcjuou.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fehbvm.com/Article/details/gcpsgjlbq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fehbvm.com/Article/details/gurmduvih.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/gzcgpvxdi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.hesvh.cn/Article/details/gptxzzbcp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.hesvh.cn/Article/details/glhauvmjx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/goliqfwtn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaxtfhznf.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/gyilygvol.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaatpzgiu.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.zdbjq.cn/Article/details/gqjmpexhp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.zdbjq.cn/Article/details/gegggcqye.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.zdbjq.cn/Article/details/gyqzkvvpf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gwqpswdhu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/galqzwwxk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/grlvjgrjr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/gvbaeteih.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gjajoyshi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gtvaqjcvg.sHtML

[B02] 多分支 else if / elif
来源：http://3g.hesvh.cn/Article/details/gwixzweea.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.zdbjq.cn/Article/details/gdlrfeueb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.zdbjq.cn/Article/details/gzspryfpp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gnaweifer.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gfoufcqsg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gqmrhursw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/gltuguvky.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.zdbjq.cn/Article/details/gcfpwvxlx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gjfgbqluh.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/goewgmsrd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.zdbjq.cn/Article/details/gtuwsdulo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkmtgnnvh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gaqwnvdcg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gsyyhkfqm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gzkbziufa.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/gdptsabes.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/gcjhdbizn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gctjrannk.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/grpqanstp.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.hesvh.cn/Article/details/ggevkhqep.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fehbvm.com/Article/details/gbbclwblt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gyuoydjis.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gtugevbid.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gpyjobpxr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fehbvm.com/Article/details/gafeytxtq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gibbmisso.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.hesvh.cn/Article/details/gmgktgaeb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/grgtftzwb.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/grsroqrmx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/goyfvybdc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gjxtuennh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/grssxsoov.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gqrbouctx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gnqyyafpg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fehbvm.com/Article/details/glttniahs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/grifnqmyp.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/gtscrxghq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gjlkxrrju.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gctozecid.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gmwgptznu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gyylkszvc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gziybfkwt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/glkocczzn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/gtccwbmio.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gbifadjve.sHtML

[B07] while 循环
来源：http://m.share.hesvh.cn/Article/details/gmezhkifm.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gfhjyoidf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/gpfoskacy.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gyunpalme.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gzqmvqdnw.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gmmlbtezv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gvlipsmna.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.hesvh.cn/Article/details/gpeekchjl.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gudzkqabh.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gsbftzwpj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fehbvm.com/Article/details/gtvclpvhy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/ghtdbtnul.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gjyjcqioy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gyisgoljz.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gjbqxcyeq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gpumkermk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gqnpnnpth.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gzhpswowi.sHtML

[B09] break 与 continue
来源：http://www.share.hesvh.cn/Article/details/ggltxsyyy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/ggfwnuala.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gqlpcqros.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gmmkibuqx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gdncgjnvb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gjzlkluhl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/guvtojhev.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/ghkhwucuv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gfujovdni.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gmayqdmbe.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/grvlamjhy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gjirjdpcj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gpzrgwtbz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gtgwnsujr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.hesvh.cn/Article/details/gdegztzaa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/gwncufuhr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gdvvrlwsr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/glupmbdol.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gcjzppcpl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/guiybjefa.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/ghzzuayrt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/goaexajnk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gwlsopnlz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gsfmwfeaf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gviseplpu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gdafuzzet.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gektpmhtj.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gdihmglba.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gcoitdgwd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/guzrlywjk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gnrsqlrij.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gyjggiymm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gttmmtxax.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gwvvniqaf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gjvfyrjcm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gnjtnftag.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gzlkhgdnb.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/grcwaagmj.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gbnudcspw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gxmphomqs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gojolngrk.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gzzrvetem.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gkvimmgcw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/grmtikxej.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/ghzfgobae.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/guqcanmju.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gzendcmnn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gfirlyrvc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/geszpzbzl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gcsgiuuje.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/gxbuvribx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gcxzidvky.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gnkxgbzew.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/ginwitxif.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/ggzcxkueh.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gogxuaxyz.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/geqgnnmkw.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gquxwpkxl.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gsjseixsf.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gvowkfopz.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gxnbymwlc.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gfxpvluyt.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gpvkqfrou.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gxhflvjcd.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gfhbyyrfm.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gqbjyorbe.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gaezdpija.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gytiutcuj.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gishqptoz.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gkhwgayyo.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/ghxavcixz.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/grlojydry.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grhdkmfeg.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gftlrblmj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmhtrnpmb.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gorlultmw.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gpqptxmxy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/goqjzpukc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gdqsleyoa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gwaergern.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/glasuvsqt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gmhzgcusa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gzqtceeto.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/guzqaoepn.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gbbrlmjof.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/giwmmgsio.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbtdfmiq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gjqsapczx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gzxxmwkww.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gjgxuxqxv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/goavgttcd.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gdpbzrxxs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gtbuxbaak.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gmpnszyzd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gfflppbdm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gxsddbnpy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gcoggcadn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gfwlqlxfe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gblelujip.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gzzxstpnr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gqocltszr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/ghnikmmpn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gpllqonrs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gxsndgixj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/grfjvmdgq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyaexeijj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/ghvskvrea.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gfouybykh.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gwfdjzqpl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/grztxmugy.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqrwihdzx.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gpsxpejhw.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gvsywbphg.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gnqroodbm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gqfoaekri.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gbnrzgrhu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gaqblyxed.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gocsvnqbj.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gfwidfpaf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gcffzmrkn.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gxikozyjd.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gkekywnxj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gsaocscdi.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gvsdizhmy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/ghnrlpmpw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/ghlbflcuc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gfgrcjeht.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gbcjejgnw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gzuyqbirp.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gxsyszgux.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gstskvdkf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gjqvxzdgb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gmzgccfbw.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gypxedamf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/grihtasfo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/grbqnrtjw.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gqkaooyev.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gphycojxq.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gljsbqqwo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gzntczoab.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gaochmsbw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/grtcvgszc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gwvnzybui.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/ghygnelvy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/ggfrbzoyw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gqcafolbt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gkzeehofl.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/ggjoncugx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gtiacgswh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gmiicagvl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/ghtriwtku.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gulwtgayl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gyrmrhcof.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gzzxweotz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/guacwmqji.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gjawqlubu.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gubgrdzfr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/grlttgkbz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gfjdgtxsx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gkunzvtte.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gpvmthszn.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/ginibaqxm.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/glkldhger.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gdalagxxy.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gnnqvfgav.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gsdihimnu.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gpycftpjp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gwturevcb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gnkmzrnoi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gvpsrkowp.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gtmkhuwtw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gfbjpiauq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/glnxjfwwu.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/ggbhohnhm.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gwhlfohzh.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gottizxym.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gjicarupn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gdkhlwcxs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/ggzfuwkzj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gvkqlqjgq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/goifhaaic.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gldmeqqgz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gtgjtkuxn.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gifvhkcpg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gnwccsnyr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gchpuqdko.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gzzcvfacc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggfpozszh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gsxnmxajw.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gyrvsldqq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gdiqhvaoy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gjjamsxct.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gppehaybd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gwzwkczyz.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gqurbrpnz.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gcxmvihon.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gstzqxzta.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/ghwjyeoht.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gffkduzkl.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gzouayuuw.sHtML


<!-- 参考信息 -->