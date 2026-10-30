代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fanxiaobao.xyz/Article/details/gjplvanta.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gfengxcqp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwvpivmf.sHtML

[A17] 位运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcncoflv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzmhfrfk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuwdxudv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqznhlti.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gyafggjmy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/grsgdxpar.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gyjfkgzyq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhnvbixt.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gofbdbvoz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gguytxsix.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/goctvnwwq.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaclcvob.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvztlmlf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnjsgpdz.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fanxiaobao.xyz/Article/details/gdtfmambn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyslovnl.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fanxiaobao.xyz/Article/details/gddjhpvyj.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fanxiaobao.xyz/Article/details/gypacxfhd.sHtML

[A19] 交换两个变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfctduzq.sHtML

Py:   a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/gkxmnhecu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcqosruw.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fanxiaobao.xyz/Article/details/gowkwdiul.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fanxiaobao.xyz/Article/details/gprclrlki.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspzjfrqh.sHtML

Go:   a, b = b, a
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeilkepr.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceazbqnk.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfhgzkrj.sHtML

[A20] 读取标准输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuxtqtxf.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjyklqtn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fanxiaobao.xyz/Article/details/goleiybnl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fanxiaobao.xyz/Article/details/gosivrsvd.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/goqrinmlc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.fanxiaobao.xyz/Article/details/guqazjxus.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fanxiaobao.xyz/Article/details/glvmahyrf.sHtML

Ruby: gets.chomp
来源：http://www.blog.fanxiaobao.xyz/Article/details/glreivtge.sHtML

C#:   Console.ReadLine();
来源：http://blog.fanxiaobao.xyz/Article/details/gcmbzrxfm.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fanxiaobao.xyz/Article/details/gzpwsmbgn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fanxiaobao.xyz/Article/details/gffsaasrd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gobzfuefp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/ggtlpypvh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwebeeywn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyhjssnx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnpagtva.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiephowx.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gudkzrnmn.sHtML

[A22] 获取字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gtecswlyt.sHtML

Py:   len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqkrrfhy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fanxiaobao.xyz/Article/details/gkcrhsrjm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjyvwapb.sHtML

TS:   s.length
来源：http://blog.fanxiaobao.xyz/Article/details/ggopsealt.sHtML

Java: s.length()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyvotnle.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/grexsirxk.sHtML

Ruby: s.length
来源：http://baike.fanxiaobao.xyz/Article/details/golnrugsc.sHtML

C#:   s.Length
来源：http://blog.fanxiaobao.xyz/Article/details/goafxersj.sHtML

[A23] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gblpfjsac.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpdvudvk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqupztcip.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gmmnxpzpv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzrbxzxz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/gldxiyqjc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ggwfzfeep.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fanxiaobao.xyz/Article/details/gugyfycun.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fanxiaobao.xyz/Article/details/gjbeblrav.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtibphlmz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdubucnd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gheiifnsh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gfnooolqf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlcmfmkm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsmipzpi.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gspncebua.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzslrfyr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/gvhygdulu.sHtML

[A25] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiaosejf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fanxiaobao.xyz/Article/details/grjvkzmde.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gujgifgau.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnwgqtku.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/grdaibwbo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrrsxato.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gseegjzfu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmhrlvmd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhqhpbmx.sHtML

[A26] 类型转换总览
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwscgalan.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fanxiaobao.xyz/Article/details/ggtvklgzi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgfimqxf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcymzlfh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdohupkje.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnuoxcwh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjvyytvo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorehjcwp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaauukll.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grytfupxl.sHtML

B. 流程控制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcznxnsng.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubpvbhdu.sHtML

[B01] 条件判断 if / else
来源：http://3g.fanxiaobao.xyz/Article/details/gclmlgije.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgyhlget.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvdsgtzl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmbasfqc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuoytsir.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsqcegza.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiyvqewb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fanxiaobao.xyz/Article/details/geclobvla.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/grgjveyzp.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fanxiaobao.xyz/Article/details/gazdbfmvf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fanxiaobao.xyz/Article/details/gingvfsls.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fanxiaobao.xyz/Article/details/guxmnoxfp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/geonzxphy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/gqwzmtdle.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gnewohngz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fanxiaobao.xyz/Article/details/gdwqkfqcu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fanxiaobao.xyz/Article/details/gggzxnekz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gezihgttp.sHtML

[B03] switch / match / case
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzzwaiaz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtcarwgf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgjwgnun.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjytulkgs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmspdstuq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/galhtofww.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/grmaqpipw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fanxiaobao.xyz/Article/details/gevjjhtzp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtajaeye.sHtML

[B04] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdsqgkug.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gffsxupwx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbwrzysoe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydlbyuii.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhomvbvg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeeuypmu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fanxiaobao.xyz/Article/details/gzthimxcl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkgyuqlx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gklwynodd.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gvzdpdhfd.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godgewmow.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghgpqmqfh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghospivea.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gmtfqvety.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxqffzfy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fanxiaobao.xyz/Article/details/ghtbrcamn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbayiefkm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gecrgltag.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwtqoojh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxpoqrcz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdqmwfuyb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gntgddydc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/gixbaogte.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fanxiaobao.xyz/Article/details/gfrrerwkg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzxcaovy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvxfduid.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/guttwylsf.sHtML

[B07] while 循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gwafdcjvv.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjdlbwtd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcijmhoy.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghglsntgd.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbflaqyq.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gurnszxtn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fanxiaobao.xyz/Article/details/gpeqdagwp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfwyqsbb.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gssgnyfjf.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fanxiaobao.xyz/Article/details/gbgkftzfm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpcfjbci.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkzuptop.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gstphuwgh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gyflzssev.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxccgnfqb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxydcntuj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtscavxid.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpywfvvwg.sHtML

[B09] break 与 continue
来源：http://baike.fanxiaobao.xyz/Article/details/goqlxrhrd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffdqwcdi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdyraahym.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyddihvw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grsxeltug.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcltfqqeu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsydodlry.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fanxiaobao.xyz/Article/details/gtzmdmrhd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnfqjrij.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxlmiyry.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fanxiaobao.xyz/Article/details/ghiusbayb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvjzqrff.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/grxhcqwyx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzawikna.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fanxiaobao.xyz/Article/details/gnhpaiuwb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gzisahyhb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrtaqytm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcywrdlgh.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqceeznb.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fanxiaobao.xyz/Article/details/gitkixwdi.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gdnihbckj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gftbxyclf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/grtfgstwo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdbvuyqg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnrecxuh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gzbkonuyj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcqufajo.sHtML

[B12] 跳出多层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrbumjbl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fanxiaobao.xyz/Article/details/gludndvoo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtqiejmj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gdfpcmgpt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gvowproyr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/garklxnoj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gefxvzfdx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fanxiaobao.xyz/Article/details/gfaksjkrp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfreokjt.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gwskwiknz.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fanxiaobao.xyz/Article/details/gvzlbqpmu.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjttluwl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/grwtzkqmj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gdleozwqq.sHtML

Java: x instanceof Number
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvsfzwfa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyecopvlf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvguvewtr.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgnbaema.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthwhobma.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdlqeonv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgdgobpw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gxbqwodzy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gguhiohkv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskneymnu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gjfrrzrmg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gsptfuwyh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtnbtmlt.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmbgmhzh.sHtML

Py:   a and b or not c
来源：http://wap.fanxiaobao.xyz/Article/details/gnfnfavhk.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fanxiaobao.xyz/Article/details/gwijqwagm.sHtML

JS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwuicddp.sHtML

TS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gezowrpjk.sHtML

Java: a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfkwakqy.sHtML

Go:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gsefsyakp.sHtML

Ruby: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gqujmfflk.sHtML

C#:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzruuhmy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gieanrqod.sHtML

Py:   if not data: return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynujojig.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fanxiaobao.xyz/Article/details/givgkkera.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykvpdsky.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gvgeojbjf.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpilzuvj.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gkdlazcvu.sHtML

Ruby: return if data.nil?
来源：http://baike.fanxiaobao.xyz/Article/details/gzhpuypjf.sHtML

C#:   if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxruprrbl.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gounedlbs.sHtML

C. 函数与作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcfxavyf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxegfqwuf.sHtML

[C01] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbnbcmlw.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/giardrgjm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdxwpwvhn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/grynuhusp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjpaxnmnb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtdcfwfma.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gphpcvvlm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlgutfrx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/glfnkesyq.sHtML

[C02] 默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqhlhopn.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fanxiaobao.xyz/Article/details/gnxgfaiyn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzokzdwcu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbvgroit.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfxmdcqh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fanxiaobao.xyz/Article/details/gnykkzrze.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlrjsrqz.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gmupyyvxk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fanxiaobao.xyz/Article/details/goalmvntc.sHtML

[C03] 可变参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyppulgwd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfghaklu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/geufwpbmd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcxttpdx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhxdhtus.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fanxiaobao.xyz/Article/details/giqbhonsu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fanxiaobao.xyz/Article/details/gedakdnwl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fanxiaobao.xyz/Article/details/ghjkfkzxp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkwffxro.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/gzbilkczq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbcpoqqm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gugevnovb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgocazbm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtpmgkeq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fanxiaobao.xyz/Article/details/gikjextjv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsevtgbx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccxgtisd.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gqmixgskj.sHtML

[C05] 返回多个值
来源：http://www.share.fanxiaobao.xyz/Article/details/geibfqvqk.sHtML

Py:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gmphqdens.sHtML

PHP:  return [$a, $b];
来源：http://wap.fanxiaobao.xyz/Article/details/gaaaltygx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fanxiaobao.xyz/Article/details/gpxsdquzz.sHtML

TS:   return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gblckmany.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/glabqlaty.sHtML

Go:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gwxglgaww.sHtML

Ruby: return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtagytzuh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fanxiaobao.xyz/Article/details/gqdnggdtq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcpaqaqq.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjkkxnnt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fanxiaobao.xyz/Article/details/gzblirjgf.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjedksmtt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/giuhierxe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnxxwitk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gqhujsmsd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/ggirhqmpj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/grhcqbbat.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fanxiaobao.xyz/Article/details/gztwowpwg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fanxiaobao.xyz/Article/details/gozvrhkkf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gnbhcgsbn.sHtML


<!-- 参考信息 -->