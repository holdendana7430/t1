代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gzepdngjx.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fanxiaobao.xyz/Article/details/gnmlwjjhq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaqiumjs.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fanxiaobao.xyz/Article/details/grnqcinvw.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fanxiaobao.xyz/Article/details/ggwhbhyyu.sHtML

[A19] 交换两个变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxhzlyibb.sHtML

Py:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/guozspvnh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxgaeyck.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fanxiaobao.xyz/Article/details/gcybbnqro.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfhcfprn.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyylarlbz.sHtML

Go:   a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gzwahjakc.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxixnrhf.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.fanxiaobao.xyz/Article/details/gotxkfymm.sHtML

[A20] 读取标准输入
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoqoczvb.sHtML

Py:   name = input("请输入：")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsentdudy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fanxiaobao.xyz/Article/details/gkpwfphoq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fanxiaobao.xyz/Article/details/gpxwnonqs.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gqjxjdwpa.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fanxiaobao.xyz/Article/details/gomdgcjwo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfrnokeg.sHtML

Ruby: gets.chomp
来源：http://blog.fanxiaobao.xyz/Article/details/gtmadvqls.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fanxiaobao.xyz/Article/details/gomgmpvcm.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjfqsxzm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcbocwpc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gxuagzipm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwjqopib.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwedxdib.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fanxiaobao.xyz/Article/details/gjelgvrzq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gwtuakfnh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/galswsvtl.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrnqujph.sHtML

[A22] 获取字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gtltpamib.sHtML

Py:   len(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gvwvbsgod.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fanxiaobao.xyz/Article/details/ggnhfevpt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtakbwsvo.sHtML

TS:   s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gbvxzescx.sHtML

Java: s.length()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxetplsk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/guwpiomqc.sHtML

Ruby: s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgmmminj.sHtML

C#:   s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhyrqbiq.sHtML

[A23] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfesoyeea.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fanxiaobao.xyz/Article/details/gwipddemf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxkqpaef.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwqazmlj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/glezrmiul.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.fanxiaobao.xyz/Article/details/gtkeymzlg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvhiqsoi.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklttxhqq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fanxiaobao.xyz/Article/details/geyardlku.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvuyrdaa.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhtceloc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnekohmn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsnlyghl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwaeydjr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fanxiaobao.xyz/Article/details/gkmimjwtx.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/giankiffm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqojtzgu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/ghsiiyyyd.sHtML

[A25] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghdavdcsk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiczvonx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gftfrmbxd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuzdfeik.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyulmzcv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmwjjcdd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcciygyl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/geglljuqh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjrcnsvuw.sHtML

[A26] 类型转换总览
来源：http://wap.fanxiaobao.xyz/Article/details/gmzrhbfii.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fanxiaobao.xyz/Article/details/gtmpmqhif.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggflziidq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnzljbyr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fanxiaobao.xyz/Article/details/gvvwzdnxn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhlyicue.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fanxiaobao.xyz/Article/details/geusfotbo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurquizjb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlrjseyi.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwzoayjsa.sHtML

B. 流程控制
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvflyglr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbwjrdvu.sHtML

[B01] 条件判断 if / else
来源：http://3g.fanxiaobao.xyz/Article/details/gdtsyyakf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjhlharv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/govbkcrla.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsokijzf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkbzjbsd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/ghyhusvcz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fanxiaobao.xyz/Article/details/gwkypaqlu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyedhwch.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/grtnkavnl.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdusiuge.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnzsqflr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gckblcynt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gienamiio.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvhlsxtc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/ggjaevfzj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fanxiaobao.xyz/Article/details/gcyvymrcp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fanxiaobao.xyz/Article/details/gcrcskgyc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbifsudx.sHtML

[B03] switch / match / case
来源：http://wap.fanxiaobao.xyz/Article/details/gzryioyji.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fanxiaobao.xyz/Article/details/gypfxiqep.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsjhutftn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/glksypoku.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebrxbjxr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiqdnakn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geehmbxqp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppxctoeu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqbiqwlr.sHtML

[B04] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzjuvcwd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotdfiqyp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpctwmxrj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghrnpiall.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgbsiucd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glxpsifgh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwbgiirk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxthunntx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatuchzlk.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfyvjmqr.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbymyyfy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhaozjbo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gkultukdu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gndftsmbc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gaenitiqq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcssdezf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgxweufg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjecsela.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssgkdwnk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdacpfak.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnwxxmta.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfsmavuf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gaopgodkm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzudhosab.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fanxiaobao.xyz/Article/details/geiegkbpm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjvoyusv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/ggwghvcej.sHtML

[B07] while 循环
来源：http://mobile.fanxiaobao.xyz/Article/details/glhrrppku.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fanxiaobao.xyz/Article/details/geeffeuhi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjllpwjce.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcvkzdvgc.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceobnaav.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyypzrfan.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fanxiaobao.xyz/Article/details/gfsxtonvu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaozcfwq.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunsclqkq.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fanxiaobao.xyz/Article/details/gbckkzvhf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmejykaf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdxmbsau.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gekbtyxpg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjqjaamo.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gpggzmxdr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gxixomrmm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdpetwyv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gvkyiuxnr.sHtML

[B09] break 与 continue
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrvnfsbe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmobzujl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghhbuzhju.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glszolooe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkzpqneu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwevukuya.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkknffuyl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fanxiaobao.xyz/Article/details/goixytyry.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpmvbsgg.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fanxiaobao.xyz/Article/details/gtrbyrrbh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbamoslyj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgxmjgsx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gqufpxtmf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/gekbpwxjc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeebpczy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/ganzsubla.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fanxiaobao.xyz/Article/details/gmhrvvzpy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsnkwpcd.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhruvbcv.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fanxiaobao.xyz/Article/details/gltcdsxfn.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gpslqrdhl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gacrymyzl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/girvticmr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gexznjdex.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fanxiaobao.xyz/Article/details/grojsnvqo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqaljoth.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gquwmqrsz.sHtML

[B12] 跳出多层循环
来源：http://wap.fanxiaobao.xyz/Article/details/gmpfjsncp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fanxiaobao.xyz/Article/details/gnecdenzc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/grjlastxw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gebjxbfoz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyhbinmj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvbhsmiu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmaugqzgi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fanxiaobao.xyz/Article/details/gseozyyjm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fanxiaobao.xyz/Article/details/gtnknvtul.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvbnemim.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fanxiaobao.xyz/Article/details/gduwdcpli.sHtML

PHP:  is_numeric($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gooruzejj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqybiyhoz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvvpfljt.sHtML

Java: x instanceof Number
来源：http://blog.fanxiaobao.xyz/Article/details/gflcpstek.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fanxiaobao.xyz/Article/details/gbehrmfgp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fanxiaobao.xyz/Article/details/govihzkvy.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxxqaayv.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppdnkmru.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqimdgwti.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fanxiaobao.xyz/Article/details/gwzoaiqrg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlovfprv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcgtqswq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gqozxuqkq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjnyrjdu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiffwaft.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcggnbycy.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmacqwxfp.sHtML

Py:   a and b or not c
来源：http://baike.fanxiaobao.xyz/Article/details/gumsdpfqb.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fanxiaobao.xyz/Article/details/gdztvjazk.sHtML

JS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxxrjiya.sHtML

TS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gomkerwnf.sHtML

Java: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gtjmesmrb.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekpumbyp.sHtML

Ruby: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/giiovtwwu.sHtML

C#:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlqhgxrq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtgfccrm.sHtML

Py:   if not data: return
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzsdwyue.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzazxxhyv.sHtML

JS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gryqrvtpj.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gqrawvclk.sHtML

Java: if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gurcukbgp.sHtML

Go:   if data == nil { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gpdmlgdxt.sHtML

Ruby: return if data.nil?
来源：http://baike.fanxiaobao.xyz/Article/details/gkkewfcqt.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvfwhyhe.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/givpbquby.sHtML

C. 函数与作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gmttznjls.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/giervggih.sHtML

[C01] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjdkqjwcd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuduxaqk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsgplprka.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glyhlloiy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcqatzynb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/grcjhpvto.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyodazmg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fanxiaobao.xyz/Article/details/grgroeoby.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/golooqtmz.sHtML

[C02] 默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gixpoogcf.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fanxiaobao.xyz/Article/details/gzzkyntlo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbnegdwzl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtqznsxb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guosoztjl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fanxiaobao.xyz/Article/details/gsxslljzf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gilbjgtig.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuahcqov.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboqvpxrf.sHtML

[C03] 可变参数
来源：http://wap.fanxiaobao.xyz/Article/details/gggypsgkd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geriwudca.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbzinvho.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmopydkgn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrpcfhru.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gqjrxrwyt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fanxiaobao.xyz/Article/details/gdmausgsx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwmrrcdh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxkcbkhg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyfigxfp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdukplwnw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiiszdcw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzvfvdil.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/goffvvobg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fanxiaobao.xyz/Article/details/gwehraady.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfvfjpfxd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorfaqjpk.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gdhkassrk.sHtML

[C05] 返回多个值
来源：http://3g.fanxiaobao.xyz/Article/details/grtiydaxb.sHtML

Py:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gknnncnqc.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdwydwki.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfninxvlu.sHtML

TS:   return { a, b };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsabrekeg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvzwmzjf.sHtML

Go:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/glshxofus.sHtML

Ruby: return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsjjldab.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuqnhahk.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gpizjxxrc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fanxiaobao.xyz/Article/details/guzlpcsfz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gfwtkaozy.sHtML

JS:   const square = x => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gtuxkvipy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gmoasevie.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gowsubkhs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyaypvsk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeognvsw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gtvqrtbdt.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fanxiaobao.xyz/Article/details/gufjxywlp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fanxiaobao.xyz/Article/details/gsmpyobnr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeplibxd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fanxiaobao.xyz/Article/details/gvobnswzd.sHtML

TS:   arr.map(String)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbojksoxn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/guzdvzabg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fanxiaobao.xyz/Article/details/gygdshjua.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fanxiaobao.xyz/Article/details/gelponyyc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fanxiaobao.xyz/Article/details/gslheghut.sHtML

[C08] 闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gjacdogmd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fanxiaobao.xyz/Article/details/gvphsybpn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvijrbyrh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/givzicprf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghexocdxe.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guissinoa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fanxiaobao.xyz/Article/details/gcjqesaoa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gssylmwzo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpwqegjh.sHtML

[C09] 递归
来源：http://wap.fanxiaobao.xyz/Article/details/grmsnidgx.sHtML


<!-- 参考信息 -->