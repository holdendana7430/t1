代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmktnota.sHtML

Ruby: gets.chomp
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvhktcbl.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwhexjxh.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvhmfupt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fanxiaobao.xyz/Article/details/gourcleiy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpkskgre.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghmlpyqwz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gmnxqmrxq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gaehzyrsz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gsuxtayuz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwloxply.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjghpayn.sHtML

[A22] 获取字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gkveqgown.sHtML

Py:   len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtilptnkn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fanxiaobao.xyz/Article/details/gktgufhwb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjpxyjjh.sHtML

TS:   s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gkmfhatzz.sHtML

Java: s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/gwzhdxwye.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gdzjtfzxr.sHtML

Ruby: s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gwssuezhg.sHtML

C#:   s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/gfsvpgumo.sHtML

[A23] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/girwyltuo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtbzhnkd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqjfvupb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/ggvrhjxjj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcchloxux.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbkdeewl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gupfsqhqk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fanxiaobao.xyz/Article/details/gnwpwdacg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqmrnqzi.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldjqqzjc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fanxiaobao.xyz/Article/details/gmrsarfyr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtadezavr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gxndsbnle.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggabewabq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfhceozx.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gkhwwbuqd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fanxiaobao.xyz/Article/details/gyenvplte.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gpesbusgz.sHtML

[A25] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdrgcxdig.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fanxiaobao.xyz/Article/details/glrvmblae.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gbklyzfav.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggclovzzm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fanxiaobao.xyz/Article/details/ghvohhelp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gapadlabb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqrtmbjof.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fanxiaobao.xyz/Article/details/gmtadpeom.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gxhauflty.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtbeyrei.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiawbelg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfovqugg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdrwlbku.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fanxiaobao.xyz/Article/details/gcbqitxxd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/ggtetppfm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gynutmvon.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gjhojtpna.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuepppvg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqnpsodpc.sHtML

B. 流程控制
来源：http://3g.fanxiaobao.xyz/Article/details/gzvhxtlsi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnohkzohi.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonpvvepa.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gejkhfvvf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/govwtxqmf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/glsbomnmm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gllhcrdtx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gwzwpnopk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwoysipq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghndwadtr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gfkltxdku.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhvtmvsl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fanxiaobao.xyz/Article/details/gctogsasi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbhgtvej.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gpyahcfdb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gvjxeygwg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmepdgpy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsduahazh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqrblpcy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gawatzlnn.sHtML

[B03] switch / match / case
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxnbbqhz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnavjfsr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gptejzutu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfkuwkoc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjbzxdhr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqnwbkmh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyyumgct.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fanxiaobao.xyz/Article/details/gunpuebmz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/ghomlctav.sHtML

[B04] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqljbisl.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gbzwusptq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fanxiaobao.xyz/Article/details/gieqitpql.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gnaslaeef.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gujknjlpx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxoonetuj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gssjbfvsb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fanxiaobao.xyz/Article/details/giheghwsv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gswvnlpjj.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gxvjdsudn.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiboijnn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrmqpbfd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrocrhhp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdvimwfc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxohwbnkq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fanxiaobao.xyz/Article/details/gbxravabi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgdimhtf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqfrwtoz.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fanxiaobao.xyz/Article/details/gxalgclap.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdheizxxc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gowyebggy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacegtdvs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfcohpvp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkkmnziaq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbibrasa.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gndrlkeqv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwoagrcce.sHtML

[B07] while 循环
来源：http://blog.fanxiaobao.xyz/Article/details/ggnkjeybn.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fanxiaobao.xyz/Article/details/gtwhfwsnl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gckaexxem.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcokwstm.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbnpstxjb.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gagnkrwib.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdezjbjxs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhnxvvpv.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwpcfbvy.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtspbsjxi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fanxiaobao.xyz/Article/details/gpzfcmfmp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyilgruk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkypvfuvr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gzzqajdnk.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoonzwqf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gipuuucmw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fanxiaobao.xyz/Article/details/garyrtkci.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuqobjkg.sHtML

[B09] break 与 continue
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyjydrod.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/gokswzyna.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdciprra.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgrsqicj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkqoosjc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxckmkuac.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzypfqtfx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnfrrfvu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guqvlamcz.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fanxiaobao.xyz/Article/details/gyhlvfone.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fanxiaobao.xyz/Article/details/gzebyuqjy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glulfewrs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdfpwbrc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhsjrknz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbumlbixk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gzqaduhri.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwglbjeyn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gzlitrcau.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fanxiaobao.xyz/Article/details/gmziycnyr.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gguoopoja.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gslvracip.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxgznfux.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/guesiditm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/glqqhyzln.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipvnmiyn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fanxiaobao.xyz/Article/details/glpokjzop.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gxijkejjf.sHtML

[B12] 跳出多层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlmzpzsa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgxsneca.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gwovaivpp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/getcgdykc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwpjthrc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gszougmeo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfgjozve.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gxduhyflg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmikaibv.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapcrqcoj.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fanxiaobao.xyz/Article/details/guakrqifj.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcmsuduf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtdsfeib.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grabbhgmt.sHtML

Java: x instanceof Number
来源：http://www.share.fanxiaobao.xyz/Article/details/gexegqiea.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glunlvuzm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fanxiaobao.xyz/Article/details/gugdvtieg.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/gzvrmzvcu.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fanxiaobao.xyz/Article/details/galzyhodf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fanxiaobao.xyz/Article/details/gmzhkxzxk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fanxiaobao.xyz/Article/details/gcnozberr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumlyohqv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvswxjzbv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfasvnmww.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtczuuexk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/grgmbrxux.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gazaqxmno.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/gocawjgmd.sHtML

Py:   a and b or not c
来源：http://read.share.fanxiaobao.xyz/Article/details/gailctwvh.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhdbewzc.sHtML

JS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gpippmkwf.sHtML

TS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gvacvkubu.sHtML

Java: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrpcylri.sHtML

Go:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gosimwzjj.sHtML

Ruby: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/ghkrsujzl.sHtML

C#:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gdmfrpcih.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/getuorqej.sHtML

Py:   if not data: return
来源：http://wap.fanxiaobao.xyz/Article/details/gfhekbiyq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoohsdlg.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfnjrezh.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gkkvgflkj.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqqbvdzy.sHtML

Go:   if data == nil { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gyedcfrwt.sHtML

Ruby: return if data.nil?
来源：http://3g.fanxiaobao.xyz/Article/details/ggotwkdil.sHtML

C#:   if (data == null) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzopybpq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gigxvuxkz.sHtML

C. 函数与作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gourejpgu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfntsgtdh.sHtML

[C01] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpohcqppa.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gfslqsuvr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbclcfbqr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guzervgyf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgqvxweo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwocejsdm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gagvsgfjd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fanxiaobao.xyz/Article/details/gvxclexnl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyeklfbx.sHtML

[C02] 默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gsmgcxxqh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawocpruf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gehnuroal.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gakkegjii.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/giofwetan.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcdxuqxc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fanxiaobao.xyz/Article/details/goknrvxdw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwqnfkrx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fanxiaobao.xyz/Article/details/gandrqste.sHtML

[C03] 可变参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvidcjydh.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/gbxaducal.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjjojpsj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcpjjomy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdfmemst.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gyfotungs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fanxiaobao.xyz/Article/details/gansxinjy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fanxiaobao.xyz/Article/details/gpjoeouvs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fanxiaobao.xyz/Article/details/gdjuslfgf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnbwdylk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fanxiaobao.xyz/Article/details/gmktblwzy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gicxmagcl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkrymkcjk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzarnvznv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fanxiaobao.xyz/Article/details/ggbvvekol.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fanxiaobao.xyz/Article/details/gaxprqasf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqzyrxkt.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqyxlhtey.sHtML

[C05] 返回多个值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdewrjtf.sHtML

Py:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gqegdrkgh.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkukufcu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fanxiaobao.xyz/Article/details/gfzgkgcop.sHtML

TS:   return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gubwnmole.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fanxiaobao.xyz/Article/details/gsqofuzpp.sHtML

Go:   return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/grcigdbgd.sHtML

Ruby: return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govmyooin.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fanxiaobao.xyz/Article/details/geiycjuqp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeujxcdt.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fanxiaobao.xyz/Article/details/guimvpspz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcwxocgt.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfyubphn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gcmakzpnz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gsccdwbcd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gotosuhoc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnioaaegv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwjghtkx.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fanxiaobao.xyz/Article/details/gtzhgyflr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpszfcvgc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gffmpfaij.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvevmaftl.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmizdszs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gfjghyqgl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fanxiaobao.xyz/Article/details/gucnwpnrr.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjsserea.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fanxiaobao.xyz/Article/details/gewwvldyh.sHtML

[C08] 闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggthevusl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fanxiaobao.xyz/Article/details/ggalzjenu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdqsikkb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvesmvbpz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvnbfkzkw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjehmbvz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fanxiaobao.xyz/Article/details/gdfogkewy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmhmdpku.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gygwkhgot.sHtML

[C09] 递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxaemaev.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gudxsymya.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvsirbrh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gozkncqoq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/giccubspg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqrdwjuk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbjjihsb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbgkueuy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fanxiaobao.xyz/Article/details/ghwwetgqc.sHtML

[C10] 变量作用域
来源：http://baike.fanxiaobao.xyz/Article/details/ggteiulhb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxqvxpbd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwljhqyl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gslhtdpeu.sHtML

TS:   同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/grlacnznk.sHtML

Java: 方法内为块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gagfozkny.sHtML

Go:   花括号块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gueoqfzpt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/gvvtixxod.sHtML

C#:   块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gsnmjdgum.sHtML

[C11] 模块导入与导出
来源：http://wap.fanxiaobao.xyz/Article/details/gwinutouy.sHtML

Py:   from module import func
来源：http://3g.fanxiaobao.xyz/Article/details/gcxrkutxg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fanxiaobao.xyz/Article/details/gtrhqgcav.sHtML


<!-- 参考信息 -->