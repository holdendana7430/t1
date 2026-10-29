代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/grcvzuuso.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.zdbjq.cn/Article/details/gwfqpdvxk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fehbvm.com/Article/details/gtpqaxawx.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.zdbjq.cn/Article/details/gcblwooko.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/gnxvgyxmp.sHtML

[A19] 交换两个变量
来源：http://mobile.zdbjq.cn/Article/details/gccdhuyzq.sHtML

Py:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/gtexulqvi.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/govejrvfc.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/gmqcgfztf.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/geadqvhna.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.hesvh.cn/Article/details/goupkbuxq.sHtML

Go:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gutokuybn.sHtML

Ruby: a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gdqycxmph.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fehbvm.com/Article/details/gsrgrwbgo.sHtML

[A20] 读取标准输入
来源：http://read.share.fehbvm.com/Article/details/getotbtnq.sHtML

Py:   name = input("请输入：")
来源：http://m.share.zdbjq.cn/Article/details/gcjzbewml.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/gwqpxeniq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.hesvh.cn/Article/details/ghndwivys.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fehbvm.com/Article/details/gzqgpkaig.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/gnnwjxprt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.hesvh.cn/Article/details/glbnlgyvc.sHtML

Ruby: gets.chomp
来源：http://www.share.zdbjq.cn/Article/details/gmmfonorb.sHtML

C#:   Console.ReadLine();
来源：http://3g.fehbvm.com/Article/details/grybwzatw.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fehbvm.com/Article/details/gztkvvbry.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fehbvm.com/Article/details/gvowomtpp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gbiijoqtc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/ghfvhumma.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gphygpxeh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gujnbyaku.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/glahgkvrz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/goznalrdo.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/gxpxfccfn.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gmdzdfjni.sHtML

Py:   len(s)
来源：http://3g.fehbvm.com/Article/details/gvllomzbn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.zdbjq.cn/Article/details/grimwjymr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fehbvm.com/Article/details/gkrbwkphr.sHtML

TS:   s.length
来源：http://mobile.hesvh.cn/Article/details/gpctvfdoc.sHtML

Java: s.length()
来源：http://3g.zdbjq.cn/Article/details/gqgllcwow.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtikewpoz.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/gybqpnpgr.sHtML

C#:   s.Length
来源：http://mobile.zdbjq.cn/Article/details/gqmvsrmcb.sHtML

[A23] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gceumellv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.zdbjq.cn/Article/details/gxqptyojg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fehbvm.com/Article/details/gsafiarkg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gqaxwnumu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gwckjzbah.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gjljcxrgd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/gtxiqbwbd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fehbvm.com/Article/details/gyhavdhyf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fehbvm.com/Article/details/gmoolrffn.sHtML

[A24] 去除首尾空白
来源：http://3g.fehbvm.com/Article/details/gxprevtty.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.hesvh.cn/Article/details/gvjjxlmrq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fehbvm.com/Article/details/gnshdgfbe.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gdkwvlmyl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gdlljxria.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gvpqsqivu.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/ghfkyvrcd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.zdbjq.cn/Article/details/gyqsoqibh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.zdbjq.cn/Article/details/goecxswkb.sHtML

[A25] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gcpmoapxr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.hesvh.cn/Article/details/ggqfgvfwu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.zdbjq.cn/Article/details/gestthopn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/gpsrbmbox.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtmwpqkz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gisijcoxv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.hesvh.cn/Article/details/guftlhycn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fehbvm.com/Article/details/gidpohwfy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gsplzxjsg.sHtML

[A26] 类型转换总览
来源：http://www.blog.zdbjq.cn/Article/details/gmyehyrsp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fehbvm.com/Article/details/guxportsx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/gpfauvndp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.zdbjq.cn/Article/details/gyltjytev.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.zdbjq.cn/Article/details/gqcfnkqhf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/ggqybfenv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.zdbjq.cn/Article/details/gmcimuabr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.hesvh.cn/Article/details/gdpiiwejn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gvsoiyvsv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfbkyztei.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/gzwmnrqvj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggklsjhhx.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fehbvm.com/Article/details/glbhjkzhh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.zdbjq.cn/Article/details/gpsrkiqmo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fehbvm.com/Article/details/glcnxjslk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gtenntgmb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gnubgtdeo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gsbdykwkk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/gxcewlydq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gzmertliw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gomjznbgh.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/grkuwfryq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fehbvm.com/Article/details/gbaiooser.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfbwvdgzw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gqchvkrzv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gjzznhxbi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gajtxpgtg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.zdbjq.cn/Article/details/gbpcqttgx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gfdvblxoz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gzhkofuom.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/guwbdnjln.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.zdbjq.cn/Article/details/gclxrnofu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzgslgybk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpncfhhsf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gctjwrfot.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/guwpjjvtq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gubyumxov.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.hesvh.cn/Article/details/gtdlgsaok.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gwyibgdso.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gprhdxvyo.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/gxnkaornx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gbxdpipgg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/ggwzrtuqa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gdqjcpfsi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/gmnaknwbg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.hesvh.cn/Article/details/gpvonivzy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.hesvh.cn/Article/details/gthjtcdcw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/geffhnhmi.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gszfmnroh.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/gkgcpfmgf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.zdbjq.cn/Article/details/gobondsns.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/grnyynidj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdopbuufg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fehbvm.com/Article/details/gaqsikzdu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gxqykxtar.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gmuiqefod.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/gfjkueljv.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/gehhnlsch.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/gadgzlseq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gopthftlq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gdwvjvzwn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gtxabarfb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/ghyutcgmq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gpzfjccby.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/gcgwloxad.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fehbvm.com/Article/details/ggqpbgpvu.sHtML

[B07] while 循环
来源：http://3g.hesvh.cn/Article/details/gmummxqzz.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/gxahnmyeo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/geuhgqmge.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/ghqwxjlxc.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gkjiigftu.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gspmvfhun.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gqzoipnsw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.zdbjq.cn/Article/details/gtnlwhvab.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/ghjyhryoe.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gvydkxela.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/gchryfnsa.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/ghwawxfho.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gkgrwbnef.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gucunmckz.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/glichidxr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gmutzbqln.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/goqhfmtrc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gvrvpindp.sHtML

[B09] break 与 continue
来源：http://www.share.hesvh.cn/Article/details/gucnijtom.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gedmjhfow.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gxzcnanyw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gxmngzovg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/ghldepcfe.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gdcojqeev.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gnlckyyso.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gcluagroq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gfnjwjbjd.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/giibrglix.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gwmfdqsgb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gvcvxzgyt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gyfdczmnx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gifpquutj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/guztyiken.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/givylkixv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gegdxxukr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gfhmgpwcc.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gcbwwfzsh.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gqkmdelix.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gxywgovek.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gcvyennvn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/grqrxhhkv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gxfatedbv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/gysyzbpcv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gvondmryv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gbgjezhjp.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gsprccygy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gzlmykesf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gfpgslqmr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gbluyaabj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gznnjdpzk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gdotfogao.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gkxsskyei.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gxsqdtbpi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/ghtpgafuy.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gefekxtuw.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gcxwmkyae.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/guzradzrl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gkjvwbluo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/ghbtuqqbk.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/ggsztonir.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/gtrnqjxud.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/goidixjab.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gbxxrvggp.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/ghpslwrbz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gtsoauvku.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhcrulcz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gvcxfwufj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gmheofkfp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gxffbhcxz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gdjaqqgnh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/glrbmwldm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gfnabvqdo.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gcnvemunu.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gvrvmmtbm.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/gqpowzsvv.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/ghgfqvwtw.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gkkbscicq.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/ggwxfeygs.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/guhjcwdne.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gurbykgvr.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/grsthqkjq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/ggglaypjx.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gfejlwmpr.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/grtscenjk.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gpllgqxnt.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gupmauvln.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gpugeitez.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gyabxxogk.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gueejqxai.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gdoibzrfi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbbxzfcwi.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gznyqezcv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtkbeuzua.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/guuporlns.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gywvaeduy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gbhynsumw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gpsbrfpqg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/guukxvdrd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gkitaoegl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gfxqmtdfp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gijayodxp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gwigympqd.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gpxocqdcl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gezelbzuw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gcbfxncxq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gxqdbkrwn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gvepcgbqu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gbwssvfrv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gsmwxnmai.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gulemetyf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gcvmzfhmg.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gdiatyvit.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gbvyzsglf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gremvdiez.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/giistuiqc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gygexvmiw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/ghoxggpnd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gjirvetll.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gcoynkpgu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gsvslhnpl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gqrbexgmy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gasgqyttj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gwfenwmvu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gbubexqbi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/grmunzvph.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gvgkyizjb.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/ggtaxppho.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gjigvufib.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/grdguhdls.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gvpcnrivn.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/geibhcwsl.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gnpleoaui.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/goaafjlik.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gepboxrum.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gsgffgelh.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gyopyilqn.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/ghyvnzwul.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gcajfwvtv.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/grtlkdhrn.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gbamwrisy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gfprchyaa.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gajtjgnwn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gajqsnada.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gsskdoegg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gwbwdldbr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/goltkwefb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gjgdcucse.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gqasfosaj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gxirhrxop.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gnowebiif.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/glolfvfoo.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gksjmxzkw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/geqllzqls.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/glnhlnlje.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gbacwofsh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gjxyumhjj.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gbknxhmis.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/glwucowik.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gvvgxnwxa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gigvjtkis.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gnbqhvula.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gqenpnunf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gguzejcpt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gytcxxcti.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gxopfyxmq.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gdedqxmgl.sHtML


<!-- 参考信息 -->