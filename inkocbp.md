代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/glnxbrgef.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gucnguxfp.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gdqkwcbxy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gslrfeeta.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fehbvm.com/Article/details/gjctexmfj.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fehbvm.com/Article/details/gpieszkyp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fehbvm.com/Article/details/gzwhljgav.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fehbvm.com/Article/details/gmevxwjqk.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.fehbvm.com/Article/details/gkfegbwpi.sHtML

[A19] 交换两个变量
来源：http://3g.hesvh.cn/Article/details/gxkzbfzmz.sHtML

Py:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/goesskeze.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.zdbjq.cn/Article/details/gfeaqtqdt.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fehbvm.com/Article/details/glbmunrcr.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fehbvm.com/Article/details/garrngxqu.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.zdbjq.cn/Article/details/gworfexzg.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gouyykagk.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gaatlrhgn.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.zdbjq.cn/Article/details/gisaetrbg.sHtML

[A20] 读取标准输入
来源：http://www.share.hesvh.cn/Article/details/gwwxwilvr.sHtML

Py:   name = input("请输入：")
来源：http://blog.zdbjq.cn/Article/details/gqoveadkh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fehbvm.com/Article/details/gawwrkxni.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/gxxkjonmt.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.zdbjq.cn/Article/details/gvrbmbpnn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/gyzhzyqpc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.hesvh.cn/Article/details/gscxtwfkm.sHtML

Ruby: gets.chomp
来源：http://wap.fehbvm.com/Article/details/gjqrbtkwr.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fehbvm.com/Article/details/gedbfyaxb.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.hesvh.cn/Article/details/gulwzzfce.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.zdbjq.cn/Article/details/gmnbmlwzo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gobwgzucz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gxbczddry.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gadtedtdr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gzygmxwug.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gijwebuvy.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gwgubiadj.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.zdbjq.cn/Article/details/gcvlxrwpf.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/gmeuitvln.sHtML

Py:   len(s)
来源：http://www.share.hesvh.cn/Article/details/gtvysknzw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/gjmracqwc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.hesvh.cn/Article/details/gcfhbegiy.sHtML

TS:   s.length
来源：http://read.share.zdbjq.cn/Article/details/gtbgplkru.sHtML

Java: s.length()
来源：http://m.share.zdbjq.cn/Article/details/gnhaadfgj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gltspceks.sHtML

Ruby: s.length
来源：http://3g.zdbjq.cn/Article/details/gpyxxmgvb.sHtML

C#:   s.Length
来源：http://read.share.zdbjq.cn/Article/details/gwxvnevzh.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gwnwjgxwk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gcfoxunrx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/ghmgvgmus.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gjddaamrp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gddbacutw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gojgxtfpk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/ggzuljxvr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.hesvh.cn/Article/details/gugbksiuo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.zdbjq.cn/Article/details/gaufoygot.sHtML

[A24] 去除首尾空白
来源：http://baike.hesvh.cn/Article/details/gwwemnkiv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.hesvh.cn/Article/details/ghvpyridk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/guqidzeed.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gfqctulki.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gjzphiaim.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fehbvm.com/Article/details/gnvbiipfo.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.zdbjq.cn/Article/details/gqqbtdltk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.hesvh.cn/Article/details/gkymhgoae.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gifpnzivd.sHtML

[A25] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gfvfskkfr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fehbvm.com/Article/details/gjuoqfvei.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/ghzkmjkzv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gbwiexatp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gneucdoab.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/gzmomynxy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gepcgddkx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fehbvm.com/Article/details/gnkggjvyl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gmapbzozd.sHtML

[A26] 类型转换总览
来源：http://blog.hesvh.cn/Article/details/gbneyqowm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.hesvh.cn/Article/details/gkbvccplq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.hesvh.cn/Article/details/gshrjmmeh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fehbvm.com/Article/details/gfpixooqz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.hesvh.cn/Article/details/gqllswlgn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gcypqucjc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/gzfupvnge.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/grnfojnsn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gcodozupy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmdriqgnh.sHtML

B. 流程控制
来源：http://blog.hesvh.cn/Article/details/gdjeyddii.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvaluzpjt.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/gejrynpzp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/gaqhylzju.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.zdbjq.cn/Article/details/gttjigjol.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gcdmkngmk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gwoeiagcm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gsbjjpzdk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.hesvh.cn/Article/details/guwcnismd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/gnogzhrau.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gdarfchcn.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.zdbjq.cn/Article/details/gdoweazqm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.hesvh.cn/Article/details/gevoemsqx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/gblvhcubp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gleasktyb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gpsnznasf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gjeuyvbmb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.zdbjq.cn/Article/details/gfkqeddkq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fehbvm.com/Article/details/gnlseyamg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/geaubsfgu.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/gganpvndg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/gggulkgbq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gobivbxrg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gyjhznqwf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gllpxpoim.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gupgxqjar.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/ghuabsvub.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/gedreaffq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gqucrnfty.sHtML

[B04] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gqgoyuklm.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/gojxcmunf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/gowjibqgk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gosfeekqb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gqtvwormt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.zdbjq.cn/Article/details/gwrvrzxny.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/ghkbwukaa.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/ggrdwjlju.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/ghjqtswuw.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gvprsxynd.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/ghuvqjqlj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/giiygtydh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gyzvtahba.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gfbcqebmr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gazlqputt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/ghkgjulaq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fehbvm.com/Article/details/gjjkcoqrz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gvsvzownt.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/gqmpldfhy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.zdbjq.cn/Article/details/gezqvlose.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gjvtbewsh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gikwdzzgx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gwifqvobn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/gqrgycirf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/gnbtmgnmi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gifvdcotq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gnpqxeomv.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/girkgonft.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gijinfpez.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gwdauesyh.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/glbrlxozi.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/grmrdvzzb.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gyyktwvdx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/geatexnui.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/gieduahrt.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gtugvuncz.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/girruqqmr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gsvezdmka.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/ghoakuniv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gljvsdmyq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gtodtqgve.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gdqkofnyz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gxhpjrylz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/gwgppuira.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gqfquzcfo.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gfldylyta.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gtzdtiqqr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/ghfflqrbf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gwfjriubr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gynzldadb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/giyjpuvgb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/garuwujre.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gxctqvefi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gsmoxctvk.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gpobssqop.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/grxhavihi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gnoxgjarp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gikuojoqw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gitzsgura.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gdlndxanz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gznvzxbwi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/guduanced.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gyqpkwfyh.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gpqfnzzpj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gntwlqkft.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gflnevhiq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gtthnzjnn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gzjodkyhz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gpsqbjbsl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/giyluphml.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/gbfxnzdqw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/glmveflxn.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/glwnbaybf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/guyprlubr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gtkbfbvgw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gfmedsduz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gfrmcrgch.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/geoejrdzr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gasxebvvm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gmraiydfj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/grqicxusj.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gjkzsjcbz.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/grlwxidin.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gfkydscfj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gsoawrhsx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gaunvikcw.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gtssyaajz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gzpagxbav.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gkpmdyrqw.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gdbensqrs.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/glbyrrflp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gfqjpflpp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/ggtovqvwo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gdbrjlwmi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gruchppfa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gclmqqbuj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/ggqhiusyn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvedsazom.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gupwuveyv.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gmfonyznm.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/giideuuzt.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gubcpopod.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gfdstilay.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/goyakramb.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/goyxjtwbo.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gslawrode.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gosrpuffq.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gffsuwjsx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/girwdjlne.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/goxghkcrp.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gvdnpgbco.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/ghxbrserq.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/guaupfych.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/goewwryie.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gmjipimbh.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gkrhmfdfr.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/ghxzokkeb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwoxegcep.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gwtjvvxgr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gluhedjyp.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gahelsjsh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gefximpdt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gnskatrur.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/grrptmdqk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gsehkomdz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/guxxzcpou.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gwghotzpg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/giigcvjdk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/ggtbetdzz.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gaxhejaks.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/ghavebjbg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/ggtlmzlwj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gifoiiunb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/goxtsowow.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gafwzrouw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/ggactoyen.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/grawovnjj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gttzlilsm.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gthhrlyzz.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gpsttafzu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gcvcgcuaz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/grhgaihyl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gzotybsvn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gsywgoeai.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/glhxnzcbe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gxcqqvhqd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gjcflngxe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gcmhtyllx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gqsoqavuu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gvyablclg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gjpjwvikv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/grosgxcvm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/ghczebgzr.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gyojnblds.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gcneuqfdc.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gotnyihlp.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gjvfuoerp.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gmbkrbidq.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gtwfedwra.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gyxzjvzca.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gcukmlyyb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gfkrjlpgw.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gzyadnrfg.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/grfgisnme.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gdlwsgcsm.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gjgsdgrjl.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gfvrtwtns.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gcexnjyln.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gybexmjhb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/ggoqdtzfz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gqhqyyjgj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/ganmnzeal.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gfnrodboe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/giensobsc.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/ganuiwluh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gpdhzxobm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gaesfggxe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gdstkldad.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gduhrcdwj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gpwdyrvra.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gijnnrqqi.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gcdlhlmic.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gvjjuxsnn.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/ghyqhishg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gmwfueuns.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gblvhicgz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gqrnsevqu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gzlbdxwvs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/glebakslq.sHtML


<!-- 参考信息 -->