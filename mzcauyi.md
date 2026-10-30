代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/glqfodnmd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gnbcnpsmu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gbahihqsv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/guxzpfmfb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/gcthrlaex.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/gbuhyqont.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/goaivdect.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gsculwxpk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/gbdyycpny.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.hesvh.cn/Article/details/gszqwliqs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.zdbjq.cn/Article/details/gcsesjujy.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.fehbvm.com/Article/details/guqxktxhm.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.hesvh.cn/Article/details/gbaxzhvgu.sHtML

[A19] 交换两个变量
来源：http://mobile.hesvh.cn/Article/details/ghysgqewe.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gsnbnuxmu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.hesvh.cn/Article/details/gdgftftpz.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gwtqtzmpp.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gvsjowgqr.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/gnsdaxcto.sHtML

Go:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/godlkiqal.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gxsbjxwvt.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.hesvh.cn/Article/details/gslhvnekx.sHtML

[A20] 读取标准输入
来源：http://www.m.share.zdbjq.cn/Article/details/giaqktwri.sHtML

Py:   name = input("请输入：")
来源：http://www.share.hesvh.cn/Article/details/gvdovixai.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.hesvh.cn/Article/details/gozvpjdtq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.zdbjq.cn/Article/details/gbztgaosm.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.zdbjq.cn/Article/details/gsanlghkq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/gsqbflefk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.zdbjq.cn/Article/details/gfkstgplo.sHtML

Ruby: gets.chomp
来源：http://wap.zdbjq.cn/Article/details/gbynlbqxn.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.hesvh.cn/Article/details/gfpmonvbd.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fehbvm.com/Article/details/gxvftebfh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.fehbvm.com/Article/details/gpburrwwh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gbnefyuyt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gcsjnthoj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gskimzxjk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gwozrschp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gwevwwdpw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gputwxkgb.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.fehbvm.com/Article/details/gjwbahmsk.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/gbeayhisg.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gpsgnxpkh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.zdbjq.cn/Article/details/gcnygdmwi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fehbvm.com/Article/details/grhxvhecf.sHtML

TS:   s.length
来源：http://blog.zdbjq.cn/Article/details/ggbfqktdc.sHtML

Java: s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gvwrvtuno.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsgqildmu.sHtML

Ruby: s.length
来源：http://3g.zdbjq.cn/Article/details/gawbttujq.sHtML

C#:   s.Length
来源：http://m.share.fehbvm.com/Article/details/grzgwjoba.sHtML

[A23] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/glxhcanry.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fehbvm.com/Article/details/gjhzrpcig.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fehbvm.com/Article/details/gbwrwvbli.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gghnfcxrl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/grnzemczw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/ghtmwunhf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gfdvqzhwc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.hesvh.cn/Article/details/gjczzcshp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.hesvh.cn/Article/details/guzktxqkd.sHtML

[A24] 去除首尾空白
来源：http://3g.fehbvm.com/Article/details/grafieuhf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/gkzsgwnsq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gukximzda.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/gxseunlli.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/grpnkwbug.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/gigarcmtg.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.zdbjq.cn/Article/details/grjpnxluo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.hesvh.cn/Article/details/gcvyetsjf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gdvawtayq.sHtML

[A25] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gmyvhtqlz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gdtrhcatd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.hesvh.cn/Article/details/gczzkdrii.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gnomimtsi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gruebtdos.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/ghuugajmh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gadofmeoc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.zdbjq.cn/Article/details/gzzikpcic.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gzkdhyiur.sHtML

[A26] 类型转换总览
来源：http://www.share.hesvh.cn/Article/details/gobqeuqso.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fehbvm.com/Article/details/gyqwjwuhg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/gcsygcvms.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.hesvh.cn/Article/details/gzwefapnf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.zdbjq.cn/Article/details/gbptakhlt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/geyohjefm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fehbvm.com/Article/details/gwgxmigry.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fehbvm.com/Article/details/gyrctzlrt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/ggquwefdk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gezdjqkjp.sHtML

B. 流程控制
来源：http://3g.zdbjq.cn/Article/details/gdlitwohm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdeetbsmk.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gpmjjdhqx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.hesvh.cn/Article/details/gyvkfonni.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gzxetphdh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gpuilonsr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gmrqgdjlt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gmgaatrcz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/geiwysjjj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/gvsafahvf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gixgdhzcy.sHtML

[B02] 多分支 else if / elif
来源：http://baike.hesvh.cn/Article/details/gxptblxpw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.hesvh.cn/Article/details/gxbkqcrqq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/gzfpaglcx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/ghsjaaznj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/guckvnrob.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gewlgbqrr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.zdbjq.cn/Article/details/gyofnwqqx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fehbvm.com/Article/details/gqpjfxmaj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gdahbbyio.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gblnkyfea.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/gqnfopnmz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gfkvfhbqx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxxeuaybb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/grtbdfhpo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gcqrqffsj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gjfodvxqw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.zdbjq.cn/Article/details/gcjukjnno.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gihmjdoed.sHtML

[B04] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/giabrwnwl.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/gweztwidc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/gkppezkuk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gvsbqstsf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gmpnlxebg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/geneszwux.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.zdbjq.cn/Article/details/gzvwkysnl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gwnsmuzog.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fehbvm.com/Article/details/glvvwjwyz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/grzfmvgma.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fehbvm.com/Article/details/gyvcpvdkc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/glzoqmnnh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gdvuimozf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gyvzfleki.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fehbvm.com/Article/details/gnyyybjyv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.hesvh.cn/Article/details/griqxswpk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.hesvh.cn/Article/details/gaqkhltnb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/gifuodzrc.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fehbvm.com/Article/details/gqoizftsx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/gtddnokza.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gxjrtjpgw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gwdqstkgw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/ghxsywivj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/ghrymlzww.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/ggnyowkwl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.hesvh.cn/Article/details/galokhwkz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gnescigjc.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/gsumgrmhk.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gjxyyydci.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gvgufwpqy.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gyhorpcxo.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gciujokhj.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/ghzfwrnvd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gefrlcnqn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/gspbbkhhi.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/giibnnlxg.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gmynatvwo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/guabijolo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/ghimeveei.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gytwnynit.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gqdidynob.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gunjqaybn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gvobhhqhh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/guhxpylqg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gxtcgsrqt.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/gtwzoxhkn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/genkqdzpv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gfmjpaead.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/glucuzfwz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gqyhrdudu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/ggmpnczxl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/getpgtkmn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gquohfjke.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gkatbhraz.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gtjhsywih.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gsiikzlbx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxvrcxqvu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gpgcvhusd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gfnchgxpn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gpgtkksbs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gddhksjah.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gzcajctef.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gbrmikefw.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gwxfceytu.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gptbxikuy.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/ghcklkzog.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gwsyxahyw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gmxamhlok.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/gkofhmeib.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gppnoyjur.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gyqogmfid.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gvpmdxukm.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gdbrrslnb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gjqxpmaff.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/guaxxjnkq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gssdcauxu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/grmxlccsz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gjbfykkfz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gmkcbjkan.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gmoialqaw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gtfekgvrw.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gkkldqttc.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/geqekbaxc.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gwgoltedz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gdrwyfbvl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gzchyufjt.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gkljlwxwi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gipwypftf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gpwnkvxnk.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/ggsixoejz.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gznjzdixm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gqlxeoihz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gbtcagjia.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gxvyajyke.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gyjbxvmva.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gmxiwcrjx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/getagobdh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gsvvaxury.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gdzvxniro.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gqtloecfn.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gwvygtoms.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gqyhjkudv.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/glpemkcox.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gbuqyzobk.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ggngcerkx.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/goljztvxe.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gcyffzyww.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gbduxbzwc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gdulxkchc.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gybmwxbgy.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gqacxzgoa.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gpiuhfxld.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gxbmqmemg.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gpcdvuiud.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gkxjbpnfs.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gfelmyxwc.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gqbdjjhhq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grujbsyml.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gqybbdvxb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gebrskywl.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gvpbmychw.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gbdzklkgy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gyjzravju.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gyisglhre.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gpmlqsvzg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gfkffngfv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gbohimcob.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gtaafxbpj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gqslkluus.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gwpypyqco.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/ghaldodwy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gpiimuikh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gngkywjbe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/giewlwurl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gsgsgwaoz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gdfmylsvm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gatbpesny.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/ghejvgccl.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gffrvmezl.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gcmhkyokq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gujvxdbxo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/ghruehvie.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gpsdnqhlj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/ggttqyuao.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gleazycna.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gfdvstqxu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/ggxywsqdt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gkoqctykd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gbakkwqxs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gucqtdstl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gfcfggaou.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gjuujwuvh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gomcrfair.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gexskethz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gmgqqukev.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gwkyqliur.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gzhrsswxs.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/guhgtmwnh.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gewttppax.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gzwwliygd.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/glfmzchlj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/goaeeoyxq.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/guekfbtwa.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gchaugdha.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gqwxkjskr.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gbvaykrve.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gyrqjqgko.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/goakqjtcn.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gkhynfelr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gkynkyhju.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/grthhrjzj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gzsveanmg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gjafbciej.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/glvucprku.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/ggknykhfo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gjnhqqelj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gcexbinft.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/grdovkjpt.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gqjhvzwsq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gaslzrkgm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gpnbhhjjp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gmmaryuof.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/geuxzcjen.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gfycmtgib.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/giahyxfnp.sHtML


<!-- 参考信息 -->