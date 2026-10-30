代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.zdbjq.cn/Article/details/gumqirlip.sHtML

Ruby: gets.chomp
来源：http://m.share.fehbvm.com/Article/details/gditnidnd.sHtML

C#:   Console.ReadLine();
来源：http://baike.fehbvm.com/Article/details/gvaeijfvz.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.zdbjq.cn/Article/details/gopulsfgp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fehbvm.com/Article/details/gitbeciaq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gylntzaqz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gqlooczrk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gspxtxvfg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvcxxaqk.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gryqpdknc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/ghablhnly.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.zdbjq.cn/Article/details/gdvdoyqgy.sHtML

[A22] 获取字符串长度
来源：http://www.share.hesvh.cn/Article/details/grzzmjvqx.sHtML

Py:   len(s)
来源：http://3g.zdbjq.cn/Article/details/gialndwwj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fehbvm.com/Article/details/ggbsiyinz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.zdbjq.cn/Article/details/glsvctsst.sHtML

TS:   s.length
来源：http://3g.hesvh.cn/Article/details/gijrjueem.sHtML

Java: s.length()
来源：http://wap.hesvh.cn/Article/details/gnsyvvcok.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gjaddgqhs.sHtML

Ruby: s.length
来源：http://www.m.share.hesvh.cn/Article/details/gqkagqchk.sHtML

C#:   s.Length
来源：http://read.share.hesvh.cn/Article/details/gmqwbqlug.sHtML

[A23] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gvrfttivg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fehbvm.com/Article/details/grhaunjpu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fehbvm.com/Article/details/gwzyuwpyr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gnzoimmfa.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gsrnymfkm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gduejvnby.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.zdbjq.cn/Article/details/ghzrtmwnl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gapcyiwok.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.zdbjq.cn/Article/details/glitazuqv.sHtML

[A24] 去除首尾空白
来源：http://mobile.fehbvm.com/Article/details/gjyauryjq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.hesvh.cn/Article/details/gdifocsbi.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/gxcnpwtuw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/gkhcrglfb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/ggttstogo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/ggwavmzbj.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fehbvm.com/Article/details/gbfksrjfc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.hesvh.cn/Article/details/grodrcfbu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fehbvm.com/Article/details/gxarrliyj.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gztrnofit.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fehbvm.com/Article/details/gisyrevsn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fehbvm.com/Article/details/gpytjtfxj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/gbgabcmra.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/grecfzozy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fehbvm.com/Article/details/gijkrcmyz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gknrfsxqg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gnjsftsrr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/ghjsftckn.sHtML

[A26] 类型转换总览
来源：http://www.m.share.hesvh.cn/Article/details/gmgmzfmff.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gnvwqdlog.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.zdbjq.cn/Article/details/gcvfybkbc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.zdbjq.cn/Article/details/gziufomng.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fehbvm.com/Article/details/goelskjtk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/ghmmgxuzh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.hesvh.cn/Article/details/gttuqkiyf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fehbvm.com/Article/details/gejbbpiwb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gnxtsuyru.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glzovegzp.sHtML

B. 流程控制
来源：http://www.share.fehbvm.com/Article/details/gvjboqvig.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfttswmzq.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/gamrbdqxh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.hesvh.cn/Article/details/guenbaxhh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fehbvm.com/Article/details/grfibylgz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/grvqrkzhk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gxatznqca.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gdxrutixf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/gkuxyypmf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fehbvm.com/Article/details/gxvryalls.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gcbupsapr.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gvldokphx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.zdbjq.cn/Article/details/gzgpcyqcr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.zdbjq.cn/Article/details/gbpnhprrm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gjaearves.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gjyhdofkj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gkngaugbt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/gcqfrgidu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gytnchhvw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gsjkriomc.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/gdsyppdol.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.hesvh.cn/Article/details/gwvklblbs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gurfsfbic.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjkwjolgr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gxmusnxje.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gdmvjeepp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fehbvm.com/Article/details/goqfezyyp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/gvgtvmvfm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gcwvyuavn.sHtML

[B04] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/grfmncfvq.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gxwgamnhn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.zdbjq.cn/Article/details/gsmgtvkdo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gkfgogvmc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gzemhuhyy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/gxamlfqgj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.zdbjq.cn/Article/details/gqvagsqev.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/gfnqbvqyf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fehbvm.com/Article/details/ggwpugcji.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fehbvm.com/Article/details/giprzhypl.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gcoyiicnu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/grduvvshh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gliqktlma.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/ghysbyyjb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gucwaxvot.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvlkbnrj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gmgrjzlqv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gbkdqdwex.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gbinripyr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/gtgzzsvtm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.zdbjq.cn/Article/details/gqljpszzv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gzklfdbyt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gxdfbaxhg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/glbobixdc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.zdbjq.cn/Article/details/gkzovdeqz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gjbkowfgb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/graqcsdnu.sHtML

[B07] while 循环
来源：http://www.blog.hesvh.cn/Article/details/gwqemhzqx.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/gahbkueaj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/gqhqxbndr.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gzlxzhdeh.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gvejokhea.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbfktvbk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gtzpcnpxb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/gygxsmmdh.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gnucnuvmc.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gzqrcfvjf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/ghuvsdimy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/glzxkiugy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/grtscophz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gnpdhifuf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gzsugfkly.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/gowicbapi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gyqwhhzki.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/ghuqqgeup.sHtML

[B09] break 与 continue
来源：http://www.share.hesvh.cn/Article/details/gafeqqkhd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gmaogwhfx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gzchgtxxt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gymogxfrl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gihzlglfr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gxicjpyha.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/glhrkbxib.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gitrdqxeg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/golwfvwfs.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gnlmskbam.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gavtxegxg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gpduhyuac.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/ggklsaomy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gpthnwoli.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/glkptrlah.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gdmdjlhal.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gaoknsegv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gdzgbepqb.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gmrpzauju.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gsmoyfpns.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gthebuuwh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/glyiphzzf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gfmadxopw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmdhudumt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gkhmukcte.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gztodiqsi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/ghghnzklj.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gtxnkchtn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gqchsqffg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gckoilqgx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gdrolldqe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gptxucxtv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gdqkczrax.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gvsrpjqkh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/giszjolob.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gpnbuajct.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gdfkyqrca.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gafnkmoxn.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gwntuquaf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gtxqjjgwo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gqdpybatl.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/glcmkldru.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gyoqjgeqs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gtsdlejmj.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gcejmmgum.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gbodysbsl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gnwovlkzv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gvwlewvhx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gsjvlcrzp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gpstvufut.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gpoklrbsw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/ggciawawc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gmpcnflku.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gqsrkkbns.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gifnyprsr.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gsnnomlrd.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/glmlajaju.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/ghcsvakue.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/guatmzoij.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gajkwaorg.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ghnlofyzk.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gyuizvfam.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gtolwkcsj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gfhchjiyd.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gnavrmfex.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gdtawjuqa.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/ghggrbtxz.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/getizznfi.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gaaonurkj.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gpgcbumtm.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gvlltipqx.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gkajodrnp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdhzbbobk.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/ghttksdmu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzkhmemny.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gmddghrzj.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gtuhdgaig.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gkbgfbeyc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gukuiljdt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gyvcclbov.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gbhwexvcj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gpkhzhjgl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gpcgnnaep.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gikdjmmke.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gqaghscdh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/grgjhoaua.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gkxspcqvh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/grnpnjccw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gvcxazocr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gkgcuamji.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gfxwbqukw.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gfeygjfri.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gievtrglx.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gfgsmvnsf.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gouworfiz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gqtmovtsm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gjhnohtxv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gyopypxhm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gicayktmq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gnjsqesvg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/grkvncyup.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gpjalmsaz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gogqtdtlr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/glvsdsvlw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/glrqzhkgc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gkohyxhaf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gyowypxwv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gchnuwtgs.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gnrnvdwia.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gielnxumg.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gskoistql.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gmntqwsfx.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/ghgoxaypb.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gfzrbwxxx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gpekeslap.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gkiblmvkm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gjokuayyx.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gcigmxzst.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gmseexcpp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gfyfgkzgt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/glatvjula.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gwwbnwjiv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gvqiwakus.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/ggpuppfbw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gslgxhrwh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gkpbhfwwv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gllyhpwol.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/ghbjjkxkn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gzifeqjug.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/giqezhbfb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gxyraluhj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gmrphwsgv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/getbqgykl.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gadodlwwl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gmpgzhmli.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gehwdgmhn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gtrspmxrq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gfyruteim.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gftbtnoyt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gfbwkbmjg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/ggzjbcpxz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/grsubjpjl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/guwgofteb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gzrhjpwcb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/guxjvogez.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gzocwxfkn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gasunovcz.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gnshkdjdp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/ggdmplcxu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gnaphmltr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/ggqnukceq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gziygftwi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gdcafjvmg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gedveckpb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gddndmxdt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/ggcczmaia.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gpfkyzgva.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gjcrxqiey.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/guvqpiisv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gppgmreat.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gkmfndhli.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gfwtombhc.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gyahdegww.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gwfwuxawi.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gbfekitwr.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gvonhfmtk.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/ggqxkprjn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gqtcwblbd.sHtML


<!-- 参考信息 -->