代发 wailian999

[A22] 获取字符串长度
来源：http://read.share.fehbvm.com/Article/details/gcizgexxy.sHtML

Py:   len(s)
来源：http://3g.fehbvm.com/Article/details/gakgvrhre.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/gguxvwdkd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.hesvh.cn/Article/details/gpqvmmgsl.sHtML

TS:   s.length
来源：http://www.blog.fehbvm.com/Article/details/gfqkmooxc.sHtML

Java: s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gmrdyjdjo.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/ggnjmserr.sHtML

Ruby: s.length
来源：http://blog.fehbvm.com/Article/details/gefaikbmg.sHtML

C#:   s.Length
来源：http://blog.hesvh.cn/Article/details/gxizzndvh.sHtML

[A23] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gcinoknka.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.hesvh.cn/Article/details/gtkvwgzex.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.zdbjq.cn/Article/details/gwgkhovvv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/ggzbbmtyk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gjvchdekk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gejtguqec.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/ggykoauyn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gcuuihagi.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fehbvm.com/Article/details/geneefqlv.sHtML

[A24] 去除首尾空白
来源：http://www.blog.zdbjq.cn/Article/details/gkfmpyzhm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fehbvm.com/Article/details/gyrbxedlp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.zdbjq.cn/Article/details/gpgrmwmgz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gfubaytkt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gnqsvdbhn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gkypnmjls.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzanklnxt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/gkgyncfva.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gffgeimjf.sHtML

[A25] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gcsmrvmid.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.hesvh.cn/Article/details/gbbfkkona.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.hesvh.cn/Article/details/gngjbrglh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gqckuovxf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gbvlcfyop.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gragyyrhq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/gzeybucdi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gdwbfvzju.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gdntztnsg.sHtML

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/gbuzmcrmf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gspmkseec.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gcxhkfjln.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gylbrenka.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gohcvacoe.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fehbvm.com/Article/details/glnaamsqf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/gzuwimjru.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.hesvh.cn/Article/details/gbkkmjcfc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gemdykiny.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyxwnhaym.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/gjoufnnde.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gitcligpw.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/gotlplads.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fehbvm.com/Article/details/gspixqguh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.hesvh.cn/Article/details/gdbgkogmq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gpxmnoefg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gocswenzt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gdorbqwpv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/gzsweiklm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.zdbjq.cn/Article/details/gzqswmdwx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gaobpkhld.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/gfxnvfuie.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/gfdbqevup.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/gblyslkzb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gekdjwqpr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gjfgwiiej.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gqagiwyyt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/gtpddrqel.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/grvkkfhxy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gnlvbcbtw.sHtML

[B03] switch / match / case
来源：http://www.m.share.hesvh.cn/Article/details/gfmbnsbmp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/gkngwfnwd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gfhwzpmcu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gtchvkjrj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/grugejmha.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gmdzvmpvt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/gfbsldwqo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fehbvm.com/Article/details/guzoqgohw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gtwvhgjaj.sHtML

[B04] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gccepfmkl.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.hesvh.cn/Article/details/gapcqimvn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/grbraersd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gjgiwxkym.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gegxjbira.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.hesvh.cn/Article/details/glnvsucta.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/genrpwqut.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/gimolbajp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gbzvndlhn.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/ghsddfqfj.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gidpohxga.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/gfxoqpzrb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/goizuezug.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gcrusamvh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fehbvm.com/Article/details/gfpgdyqya.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/gfylfleml.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/ggyhqlksg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/gnkzwgjau.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/geypprmqh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gfbfgaact.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnygcozog.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gaxwskean.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gqxbpissl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/ghsztewtp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gygukqldl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gbdruwzsn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbpuzacjr.sHtML

[B07] while 循环
来源：http://3g.hesvh.cn/Article/details/gqunxjbfx.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fehbvm.com/Article/details/gqvsxlwzq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/gcwcjyamd.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gzyzshndl.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gawvkybxf.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gwkdlzjqs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gjvojkffj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gykilpsnx.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gjzuezoxq.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gkobzvqcj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gaswztzrm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gjopxywcc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gjmxgopgn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gspebudud.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/guxdxrttl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/grqksmaqm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gsbxvkvop.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gbdfcybne.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gvwwkedeq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gwzyirlou.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gsabwgtqv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gkpbeqdao.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/grsnttdds.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gnubmbezo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gindguloo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gxqepqiwj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/ghisfqrgg.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/govqblghx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gtzyijtyz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gujttnrri.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gzwyiykwo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gxdznzudx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/ghglpmzfm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/ghkncyohx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gucnxmlnd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/grgswbsiu.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/ghsxgguyy.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/gpwdikhwt.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gwkcflcyf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gaebokzws.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gvqydzgvd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/giijhruka.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gnnuwrmlo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/guoqwcxuz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/grfjnmmnl.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gkuvxvdtn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/glhtannvb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gkkojuipd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gfwhhojur.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gmnnhlssq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gyhvcyybg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gdlxyrquo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gfrepiiiz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gfjvhjlci.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gngswplww.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/ggejwmreh.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gkrhatqxs.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gzucgexxu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gaftiqzwl.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gozpnwbou.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/guzuodulq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gjafuqehr.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gmhqyuvmw.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gggzmvqhu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gnkqkqgvl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gmjyoilfb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/ggwnnmpey.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/grkhtetpe.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gebtegkpv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gazxkbxom.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gvaawdtdc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/ghazvlrfu.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gahzxfrgg.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gdpvofgyr.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gfncuptfi.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/guylewxqb.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/goclgczlm.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gqagzvjrr.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gmaubfbbq.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/grrtqstwl.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gfxvitgcb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gnxqyoovm.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gtuusuiib.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gpsbcmvxf.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gnkfaghqw.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gduipgumy.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gxjvgblnr.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gkuartcpz.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/guaqqzlcg.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gzuokxwhe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gguwmewah.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gxybkcwem.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggwqqjgtu.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gwkciapii.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/ghdunweid.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/geuvuibxp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/geynwzpof.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gvtfcqbds.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/glqrpkmjz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/grdefsywf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gzpfvnobr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gopwtjhjv.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/glrqriuwt.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/ggrwgqdao.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/geqqzajvi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjwwluptl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gxqiswcfa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gnvkjkvum.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gzowssyvd.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gauxnhsni.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gaujbpjza.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gdbxxwfvk.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gxmduhoup.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gsevosvlh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/greesdnfx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gaormkjym.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/glyzpepfe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gptwhzdkd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gkvntlhdm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gzylmlvwe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gmphqugqf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gzeetbkfw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gvmpyssor.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gtznyugwh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gmdllnazy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gdcyixmrp.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjtyqjqkr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gmdnpchet.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gtpdpuwpf.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/ggqklgbgc.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/grvzpgiip.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gmnsadhgc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gwrgfgfhk.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gwyvoliie.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gcjjmtmen.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gtdynopcl.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gndipzwhp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gjlyhrpwx.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/grbltvjzh.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/ggsmqqxuf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gwateaguk.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gdqvquxdg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gnhsiskmt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gemnolkqk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gxbatlsct.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gkrszdtgd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gbdfnujjo.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gbvjuubkm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/grawlljgx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gokwhqrus.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gdynolemk.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gqjovjitj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gpwfkjupy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gclyqiymh.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gfxkatrhq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gwhuxnmfp.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gzdssqpbw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gjkhnkbdv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gweshbvbm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gblgtedwx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/ggtwaaknw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gwcxnzqfy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gtmvjybvi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gewumscqy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gumikwfgq.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/grtffdcop.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gkcsptxyd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/grtxbhcdv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/glncpqagn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/ggautvuut.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gcuuyqnow.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/giuaoihjc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/grulogbwf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gtfrnynbp.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/ghqquilgt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gialqbirt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gzdczujlo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gtqpvtznt.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gnslssyzw.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gnmsufsof.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gtxxytzci.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gshvnaihs.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/ggjivubcq.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gtojfpdpl.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gnacfjcog.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gqtqgznfo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gjrzvwjxa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/guahpbfbz.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gxkqcoztj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gzuqstcma.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gubhenxny.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gervmxbsz.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gtlnunxzx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gkrhlyiey.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/genrhdqlx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gvafefjwx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gzccyalhw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gcdyerzke.sHtML


<!-- 参考信息 -->