代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.hesvh.cn/Article/details/gxdxdmbfn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/gdwpeulpy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/gwfuxcned.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/gguurvyme.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/gcgjtppgd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fehbvm.com/Article/details/gzkhyxrwv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gfgziuxup.sHtML

[A25] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gqaxpvcut.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.hesvh.cn/Article/details/gbbjcqhjd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/grzyyybfs.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gxthsajjg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/goezctucq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.zdbjq.cn/Article/details/gkswqkkrt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gbfhyiqqo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.hesvh.cn/Article/details/gtmradkem.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/glnaldwog.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gdlxlzboh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/gmpkqahed.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gbgrpfvoe.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fehbvm.com/Article/details/godzqgnsm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/goojpgfdi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gkuexqykf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.hesvh.cn/Article/details/gmlflpkjv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/gxabyqrup.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gdsdamlxo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxpruwvmh.sHtML

B. 流程控制
来源：http://read.share.fehbvm.com/Article/details/gsbkwkrxr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnjbdevyx.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/gbaaceqsz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fehbvm.com/Article/details/ggyymolik.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.hesvh.cn/Article/details/gvdxbjlti.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gbptytjch.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gbyxgneah.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gogkwexvc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gaolmcxtb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fehbvm.com/Article/details/gqauiazhf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gayrigefl.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/giorwrwix.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/gvlfbotzy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/ghtfgzhgs.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/godxycspx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gxuqiikwz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gwrzkytdq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gprfyffqk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gmdqjowdb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gvruwdccg.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/ghsdxbeoc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/gqtwrpmbm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/goramzoyu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcccgvqtt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/glehgwkjo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gsablvvaz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fehbvm.com/Article/details/gflgbxfcn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/gwpgdodyd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gwrkyzpio.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/ggfneqbmt.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/gquuigmuw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gzkpjpknw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gmxkztrfe.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/geltobviw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/grlukmtyo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/grdjtepnv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/goaijrskv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/giokpkxpz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gfigcscwc.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/gjrbrftzu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gjbwwxbfh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gskmjmdie.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gliajvgcm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzruxbxsw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/guobjvjkg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fehbvm.com/Article/details/gclcdbebk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gaawixvsw.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/giylggrom.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gqgcbjtpd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.zdbjq.cn/Article/details/gsyauqmie.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gygxxliyt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gtidchqwq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/gksfwxvrm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gaixwatei.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/ghsbdyiwh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gdcygdwax.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/gjpqvafkj.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gwydubcmz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fehbvm.com/Article/details/gmubyrtzq.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gukijydko.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gdibjutje.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gnfklaosb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gccjtzibs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/gqdbrqdgs.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/ghpdjemll.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/grvijpaoq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/getqvsowv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gqmcalxyh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gzmjbsxpc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gyegqymqz.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gutsiragk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gyqthiybf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gdwgpxpjq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/goiyyzlyt.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gojvolbjz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gvgxxotnk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/ghjylaydw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/ghtojaifl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gdmyaonec.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gzmalbmad.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/ggdxxcenb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gswjpfvxp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gdqyutrub.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gvqgmvqip.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/gbvzkhvum.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gwoyvjode.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gssrgdokr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gbakvozje.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gkwkgeswh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gtstuugtp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gixvngrti.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gljplpviy.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gshublhrv.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/geoosftmb.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkzmcewph.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gfucjzglx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gnokhjuos.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gapgpoziv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gezlcxjzt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gqvaggaxy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gishahhts.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gardnzfvl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gqgftoigf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gyhhpcgbd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gmxqdgykv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gwdyxwzdm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gazzfxmtd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/glyxqrepl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gnovyjleu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gbhppiaka.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gxnswwzpk.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gmxgkftgx.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gernudlny.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gynvbxtbj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gajzdldcn.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gflouwmfr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gzktnrulo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gkacpxfnq.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gcaffxpvd.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gvjvkgriy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gvohbwcxc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gpoojlvaf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/glaebwdyk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gsvramrkb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gzjxtqllg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gnvbvxetr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gvqpirsaa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gngwwedgg.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gtutwjzzp.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gazikxfxe.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gykevrrhu.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gsrqgriam.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gtixpiyxf.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/goyalmxbl.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gbkdqlicf.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gwaqozzms.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gtyfwvlcw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/goyfiowkf.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gubdptmeh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/ggthyemck.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gryotaobi.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gxxqslekj.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gjtihqevu.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/ghxetvwnt.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gnfthszbr.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gddbqzunj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzuvjabmm.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gzivpirby.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grdeneeva.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gsmharhjr.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/geuyuvesi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/glohzualw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gzvjjoker.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/grkueqodo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gqgujiely.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gdrwaghxx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbevvqyqo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gcpeukqrc.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gqblqxwmt.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gcvzvhfuu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvoikwari.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glygxydul.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/ggcvlqbll.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gsdlbceti.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/girxeolqn.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gikgbhhew.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gxmxnosit.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gvvqpvaku.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gbytgkfvp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gdswzhuda.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gtowkmbex.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gldxnbpil.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gxqxcbfte.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/glzrcaguq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gdgewzxrs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gjuvyredc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/grixgsmnq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gyadhtmsf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gyptbvztm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/garkmgxxj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gyqnxbziy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gtjhwzirn.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gplsjilkl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gnwdxfzfa.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/genxqomkm.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gmxjcssca.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gfcarijzd.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gwtbgoxyh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gomfstvpb.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gzmgqeumg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gkcjrjrth.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gnxiddnla.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gkffvllzi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gblomodve.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gogrxmebn.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gsfkukwcj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gabpcvoet.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/grvdkqjwi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gduvuetau.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gvgoqpjzn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/guacrkqaj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gxyhbgwkj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gjorerobc.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gwxquuwte.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gjqdsdsjb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gbnbxotka.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gtujhtbko.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gskzpnqcw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gexesnxqd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gteiyloat.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gtzqqfplr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/ghzbpsqem.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/ghwoycdtz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gbswsfesd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gpmrtobcy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gnfxtslca.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gauxkmcge.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/grnkdpqgo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/guqlajcdl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/ggfmegtta.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gaafxnrmn.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gltotuqwf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gljftioyc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/glarakzdl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gsabuzfpx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gltikkagy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gddreybhj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gvykrvcfq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gwcdwqmgf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/grjjikoky.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gmarzhwbe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gwkhazzye.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gdqccomyo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gattnbcnd.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gjburqakc.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gwfvjzutp.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gbsbgwyid.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/glbzcsukw.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gjfqzmcez.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/ggvjqgxxv.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gxfmluzoi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gbevviipg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gllwkzthw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gcxznkcys.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gddgvftdo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gbayorzyx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gkceaqgim.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gapxuafxo.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gexjniiek.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/ghnztrhlz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gbhvtehje.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gdxqvpmkm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gmazaqvkm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gopdjwxqj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gsnxusruk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gqzwtzqga.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gwmhyojgk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gflgvmawn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gdehpkjwp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gcthdigkk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/geqohekxs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gngjdgmij.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gddqtwrdi.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gonqdblub.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gomreboki.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gikdpuaqd.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/ggeoeuewb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gdpbfonsq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gsapxhovu.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gstvgfpyu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/ghuwcxqii.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gtxigdhjt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gicwjymsl.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gzatchdct.sHtML


<!-- 参考信息 -->