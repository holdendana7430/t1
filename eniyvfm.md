代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.share.hesvh.cn/Article/details/gokbaztmu.sHtML

[A19] 交换两个变量
来源：http://m.share.hesvh.cn/Article/details/ghdyynbeb.sHtML

Py:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/glumarsbr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fehbvm.com/Article/details/guujsmlwd.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gevsevmmj.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gtpbedwsl.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fehbvm.com/Article/details/gqbdqklja.sHtML

Go:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/goxgqjzmu.sHtML

Ruby: a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/guuibmfjh.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.hesvh.cn/Article/details/gicofulds.sHtML

[A20] 读取标准输入
来源：http://m.share.zdbjq.cn/Article/details/glkbrqmci.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/galachtpp.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fehbvm.com/Article/details/gqfmuocwk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/glwnelfzz.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fehbvm.com/Article/details/gerzhssun.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.fehbvm.com/Article/details/gxmbswyft.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.hesvh.cn/Article/details/gncfpfpxa.sHtML

Ruby: gets.chomp
来源：http://read.share.hesvh.cn/Article/details/gvadsdoib.sHtML

C#:   Console.ReadLine();
来源：http://mobile.hesvh.cn/Article/details/gfgpeyweb.sHtML

[A21] 保留指定小数位输出
来源：http://3g.hesvh.cn/Article/details/guzdwlxkn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/gxrprihij.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gopyerccj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gjlxbsqrb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/ginfjebsh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gqibwvkjy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/ggctxtjeb.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/grinzkgxs.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.zdbjq.cn/Article/details/gedlosfom.sHtML

[A22] 获取字符串长度
来源：http://www.share.fehbvm.com/Article/details/gwnwziumj.sHtML

Py:   len(s)
来源：http://www.share.zdbjq.cn/Article/details/glqqvinsy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fehbvm.com/Article/details/gvbrxczuk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fehbvm.com/Article/details/gqzvntuds.sHtML

TS:   s.length
来源：http://baike.hesvh.cn/Article/details/gwgrknrwy.sHtML

Java: s.length()
来源：http://m.share.hesvh.cn/Article/details/gvqwqwjwu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/gaidezglo.sHtML

Ruby: s.length
来源：http://baike.hesvh.cn/Article/details/gxnzyohvk.sHtML

C#:   s.Length
来源：http://baike.zdbjq.cn/Article/details/gykofiahl.sHtML

[A23] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gdmmohpjm.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.fehbvm.com/Article/details/gudwwumem.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.zdbjq.cn/Article/details/gxhlkvgru.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gkujjuopu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/geahbmigb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/guoegrcwr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.hesvh.cn/Article/details/gbahhsvie.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/gjpwmvjjr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.zdbjq.cn/Article/details/gqedyhwvu.sHtML

[A24] 去除首尾空白
来源：http://blog.zdbjq.cn/Article/details/gebkintng.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fehbvm.com/Article/details/gniagvzro.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fehbvm.com/Article/details/ggtewsikm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gxviysdgg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gttncdqor.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.hesvh.cn/Article/details/gcqrygmsb.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/gbrolsfyj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gmgrwzdvl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gqtrfuidb.sHtML

[A25] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gficzabfd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fehbvm.com/Article/details/ggkzdkkhf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.hesvh.cn/Article/details/gxbqhrwrw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gwnonfixr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gfgfustpe.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.zdbjq.cn/Article/details/gazsppfzo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gvccrqqep.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.hesvh.cn/Article/details/gqlrzgyml.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gkkpxazur.sHtML

[A26] 类型转换总览
来源：http://baike.fehbvm.com/Article/details/gjzhaycrq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gwushzbhr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fehbvm.com/Article/details/glknwcznl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/gvnqeuozf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gnxikqtla.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gbhmfmsud.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gpvbvgewy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.zdbjq.cn/Article/details/gzqcjrjgx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gcjetazsa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzalxosxy.sHtML

B. 流程控制
来源：http://blog.hesvh.cn/Article/details/gotbrovff.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gayvrlbfc.sHtML

[B01] 条件判断 if / else
来源：http://www.share.zdbjq.cn/Article/details/guazzuzku.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gsmznffvw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.hesvh.cn/Article/details/gvfhwzbdt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gplhwrwyv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gemfsjfpk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gykdydxry.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gwqdwylqp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.hesvh.cn/Article/details/gjneoppiy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gvwvivxqi.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fehbvm.com/Article/details/gfeardrio.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.zdbjq.cn/Article/details/gghwyiavp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fehbvm.com/Article/details/gheobuizt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gcqoejilz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gxjdmxser.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gswusnsod.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gzrmhiqsl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.hesvh.cn/Article/details/girqmxrco.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gkszdxsfk.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gdimcniwd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gjlbewuhg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/ggzsaodfi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gdhtenvul.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gbgihmact.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gvavauzjk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/gdgnaesjh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/gvrgdkkdx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gcrkwotdv.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gaoalvuhi.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.hesvh.cn/Article/details/gyjzjgork.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/gqjgwfjqt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gikpoydsf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/guxlbighr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/gilpvmbuc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/gwzlatgod.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/gdhelsuue.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gbvcptstp.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gpqsiovyq.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gykgotvdu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/geznjkmnk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gndsboagp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/grpmvnjbw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fehbvm.com/Article/details/gpkynmvhn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/gmtvlqgor.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.zdbjq.cn/Article/details/gbdurzzjy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gdrlplbdv.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/gvgdkrqep.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/gnadiwsbd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/grozixzgp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gwhbgjqqc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gychevoyn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gykfrgtto.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.zdbjq.cn/Article/details/gzxhjopgr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/gsypjlevb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gixuaiphf.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gywcphdbt.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/grpvlfzhg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/gtunmwbdv.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gqvuuzyxi.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/goeugyzjn.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gkxktxcjl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fehbvm.com/Article/details/geivmtais.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/guezniowp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gfzxgrecp.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gkdhxqrfw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/ghunfdlsr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gebuedpky.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gumaabchf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gbzttnqyv.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gjspcpyky.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/ghcrfsqzo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gcpwhhgrp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvpeoduv.sHtML

[B09] break 与 continue
来源：http://read.share.zdbjq.cn/Article/details/gmjeidcca.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gngpbfbse.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/ggcxudnsu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/glkyxxpil.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/grognshcm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/glqhsihbu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gphujrcjb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gcvapekyh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gwaxeblvv.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/gdatxopyr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gujlqlgwd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gcdhhsgfo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gofhffhbn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gtknpufys.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gsbvystra.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/gjhpxmyab.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gezfmsfxm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gwmtxdydm.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gkpiyemqy.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gpgyglmst.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ggixucoqa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzmakuurp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gbczdgbfc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gchongkie.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gkxmmeszk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/grymkhmok.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/gvxsqxiqv.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gnlqetror.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gjctddvmw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/ghmrjamnu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gcipkpldk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbzenry.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gkscgcrrs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/guuurysyd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/ggokoaoij.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/gmcngvfcw.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gpepujmhp.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gjneoawlo.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gmaqrzamz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/glwfyhfho.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gqemojorp.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gknmxthtp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/ggirogabz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gfzrycojx.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gggptbnof.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/guykhaecp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gktnqtced.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gqlfswpon.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gojniqbgc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gluekwuop.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gupqhbqcr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gdzblnzxn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gchocwmbu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gwtcvfyku.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gluowqkit.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gzmbfkxfx.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gkinglvcn.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gasybqpnl.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gydembniy.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gjsqwjska.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gscojmzfp.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gghgonofv.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gmzczhcgl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/giaiuuorn.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gtqaejzil.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gacheaogk.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gpmlainoz.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gahtkhnyn.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gpvmsmtki.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gvcmqekqv.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gnhethmab.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gupgfayyk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdhpyucgv.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gwxvbrmlb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcxfyskyu.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gtaywtttc.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gwdspeijj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gymyudcnh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggmhlinle.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gudlfjbnj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmpruhnrd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/ggnscsgrh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/goosrovmu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gvptrhcyi.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gwasvpfbc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/ghxtfbprf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjiikoyqz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gtyklgrsw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gqftwdtfw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gccbpxwcv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gwwyqhkap.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gbehfmcmu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gzosiviow.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gcfwqnizx.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gsgwbxgad.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gunsrmnvg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/giugwwlzs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gzirukawd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gsrhqihnf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gpvpggzmr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gqjysjjcj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/giguyxzpd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gfmozhjks.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gqijftdty.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gepgdqpty.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gsuvztyvl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/gkbcswrfb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/ggpbzrhgl.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/giepyboce.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gcfletavu.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gcedoxkmk.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gxmjpjbjv.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/ggmyubfit.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gtqthbvfv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gcrfylkvh.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gqlrslunk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/guikafpfi.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gxjjidgke.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gzjqdrjwu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gbmkuahcx.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gcxdrmysy.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gfqefqnzw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/ghxsfvirk.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gbznzppci.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/grszghebu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gudtnhbfe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gajlltmrh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gwftzvaav.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gcgxtfqsi.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gebewfdak.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gupllurpy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gtlcdhhqr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/geougpnbd.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gvupjxgnr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gupwyfovd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/ghcswlvnl.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gilgkgcqp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gxkrxbsbn.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/glsfsuptw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/grzcinfof.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gyzpmmfee.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gmznfcrgk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gqabgjvop.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/glgvudzxq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gxywxupum.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gvzqtiydw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ghcstyeat.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gxladyupo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gzqmzqohh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gdhsvdlqx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gcslsrpqo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gocyqazpo.sHtML


<!-- 参考信息 -->