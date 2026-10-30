代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gjuvpevqq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gisoevltw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gzrwzomkp.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/gnstvochk.sHtML

[A22] 获取字符串长度
来源：http://read.share.fehbvm.com/Article/details/gtykuokpk.sHtML

Py:   len(s)
来源：http://3g.zdbjq.cn/Article/details/gnpsyatcq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.hesvh.cn/Article/details/gwftqpbcf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.hesvh.cn/Article/details/gfknkilcj.sHtML

TS:   s.length
来源：http://wap.fehbvm.com/Article/details/gabqqxuqz.sHtML

Java: s.length()
来源：http://www.share.zdbjq.cn/Article/details/gtkteiynq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gijenacld.sHtML

Ruby: s.length
来源：http://baike.hesvh.cn/Article/details/gldhxmpob.sHtML

C#:   s.Length
来源：http://www.share.zdbjq.cn/Article/details/gpglpjuru.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/ghagganyi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.hesvh.cn/Article/details/gfchkuhin.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fehbvm.com/Article/details/gfpqekahh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gfapojpll.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gisrehbzw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gfusdapzq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/gkitnjgvq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gvaztzjpy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fehbvm.com/Article/details/gtahypddx.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/gpvryxlxj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/gfrjylxvx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.zdbjq.cn/Article/details/gvahpueky.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gnklwatbi.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gfxjrixyh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.hesvh.cn/Article/details/gkdauqgnj.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.hesvh.cn/Article/details/gwxqulupg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.hesvh.cn/Article/details/gpjrppsta.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gbusxizpe.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gbzzjtmql.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fehbvm.com/Article/details/grtgepeiz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.hesvh.cn/Article/details/gxbzyoynq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gpcjrizbk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/ghwnckzbs.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/gsgfvjikt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gvogssnph.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gzgmhctrm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gxethcowk.sHtML

[A26] 类型转换总览
来源：http://m.share.zdbjq.cn/Article/details/gvtpcwiwx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fehbvm.com/Article/details/gimxyjekw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/gwahzjcdj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fehbvm.com/Article/details/gblrjhpdd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.zdbjq.cn/Article/details/glqmfkrrp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gmupiafyl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.hesvh.cn/Article/details/geibrtfef.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fehbvm.com/Article/details/gnbcjduho.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gwqzibhwk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtimdbvuz.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gghnqbeol.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glqmoyjot.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/gvsqfehzd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/ghhrqttse.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.zdbjq.cn/Article/details/gbicwyiep.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gxfqqjavv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gjmcrqbhd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gexozphsl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.hesvh.cn/Article/details/gegwpstuu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.zdbjq.cn/Article/details/gifuqaoeo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gqeertnjt.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.hesvh.cn/Article/details/guoomhfyf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/gtvcrrhsr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fehbvm.com/Article/details/grnqwhzpg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gebuafaen.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gdombuvym.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gseltlqbn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fehbvm.com/Article/details/gbxjbwugs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/gclqeuswq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gaxwhvqwf.sHtML

[B03] switch / match / case
来源：http://baike.zdbjq.cn/Article/details/gmogsjmhp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.zdbjq.cn/Article/details/glulbkabo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/guhsjboxl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gmsvascct.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gzxjdapcu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gyfwrwamn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.zdbjq.cn/Article/details/gtjeaxrne.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/gtaiwxkpy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gxmrjpfwx.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gpnqjfbei.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gyenptpgs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gyolnvdsc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gydzoiphd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gaathkmut.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.hesvh.cn/Article/details/glypgepsg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fehbvm.com/Article/details/gmtlkrjgi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/glyrejvxf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gqhquusso.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.hesvh.cn/Article/details/girhhbihz.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/gqcvbkkbc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/grlkpdksu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gypjbbiwo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gnkibguyr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/ggclvcrqa.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gmhifreae.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gbphdavmx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gmyzxjvwa.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/gfmxcpgaw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/gdkypdowb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/guvwopmhk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gbaxhgijw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gikrgfcvr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gavvlvcpe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gcbymwuty.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gwwuuejvg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/ggwkioogt.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/gfcjzjmzu.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/gsriedwzf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gxoaherlg.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gpzkacioq.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/glnqfgpxm.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/geqbvwyni.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/gyzdejlbz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.zdbjq.cn/Article/details/gcekqfpyu.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gaiwhacwm.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/grnnqiqra.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/gtdfuqglo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gyvuvomos.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/genlzachb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gcruzkcld.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gabsqhcuc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gqixrwqum.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/ghaqzffsn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gpslffwzw.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/glgfxsvww.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.zdbjq.cn/Article/details/gpdseeenx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/guxdwiyjl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gbtgqyfot.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gvcyhzgfc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/grwicpuex.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.hesvh.cn/Article/details/grgbtqssu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gzafbogel.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gpbyvmdlu.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gxnlwgkpf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gpotmypgq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/ghstbslsq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gbuftmvcd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gicmcffzv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gmssjbvvn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gfbizowxg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gholizwqg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gyfqfwarh.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/ggvafpgif.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/guagfrbgr.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/gelzlcbkq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gmxiuwogx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gfsbhhmhj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gsxmrmvcw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/glqqbrdvp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gawlgxpvr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gjnxzbstg.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gljgvacuh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gkrczaaqe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gwpdndrlj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gygfuaibj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/guwgxceqt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/ghrrcmnxd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gelzocmoo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gzjuvohqf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/glgqwwqhv.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gsmilcwsj.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/gxnpgfpvc.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/ghknpwfoh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gwyfzjhqk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gxktiizvh.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gkbbfunix.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gjxbkpdhv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gzwemxtia.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/glvaiqskq.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gesqmfagv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gvlxqjhwn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gpnoedvvn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmccucfw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gkoeiqlbs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gvpninrhg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gmqsimddv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/guidzqndo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gpggkyngs.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/ggvbyzwql.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gmbdddtts.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gcawjfvey.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gfijrwtkg.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gnbegjblz.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gcpkfnpvf.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gaslffxzs.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gktbtmctc.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gkhqpwpaf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gkxgtczis.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gidjrkaij.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gadrxwkng.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gdknfcleh.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gnvdjceqq.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gtawueftq.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gaufuwsrq.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gngqmiqop.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gindaetwf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpovniwba.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gtkxgynxp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gryyekftn.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gblorwlks.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/grzbbsqxi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gofgujscv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/getiiqtva.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gtxwnnljv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gnrwafobz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gzmlscyxf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gvvfiljwg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gtylkhvog.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/goyxkovri.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gxxjjarmx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/ggwytspwl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gdyqaejnx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gsihbyehg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gvqsmplqe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gddummxwj.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/glrqkkeqy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gpylvjdfz.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gwcaihckd.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gcgpvuebr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gygzrgxuw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gwxilnwjw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gqwievphc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gfzyrekzw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gbstvnusw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gljzmoqum.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gtpymohlo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gecqxslsg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gpiqkmwbs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/ggijyftmt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gbyrimecf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/geigyflqv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gveeahlrc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gibdqnzju.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gyczqqovo.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gsaescceb.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gtdxnrsfj.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/ghgercqkz.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gjmrisbcc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/goqjikfgo.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/guytlbhof.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gskuepdpr.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gmzbsrvix.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gdqoctxve.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gvgxkbffo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gcmtdcscg.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gbxbidfyi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gcotcluri.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gjghsgtah.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gdbyqrrpq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/govupeccr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gsisedoii.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gzncgzfuv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gzfgykzfo.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/ghvbwbexi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/ghazvyuco.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gkuiucbtz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gzyscpkam.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gglmbalnn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gmdwjjpdo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/grqgifrxj.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gttfnwjux.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gjuykybbx.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gpxximjyu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gwawtrgrb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gjqzckevu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gbdwcbvxn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gfadialma.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gvwhzkute.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/giovfmozb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/geanssesi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gosjudgzo.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gdyuwlllf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gmxtkyugw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/grhybvyfk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/goejlcoha.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gzextzkbu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gvfgnhoyy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gjbzgwtdz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gvlsedhdh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/ghhkufhrc.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/grpbcjppa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gwqankfez.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/grfwnxizb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gjxrhzjfg.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gzmbcsslx.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gjrlivoyi.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ggmnyxmlo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gwvgpkqdu.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gmiilqmts.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gvkplnvya.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gbijfzqta.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gakyhtujd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/ggjxfavuc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gybpopbvz.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gtfvrgjnn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gkfclndgz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gkvpdmrrl.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/ghnxnajba.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gyxvveocu.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gmtnhwklw.sHtML


<!-- 参考信息 -->