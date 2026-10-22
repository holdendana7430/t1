代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rpfqzfcm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2poptstgo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vwpbneax.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ilrmmqus.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mnvxxrat.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2osqtkidj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xrneyezx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2uvpugdxo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2adhyqgoe.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gkjzmxgb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2xnpubgwl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qvzuxyjk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2qkmjhgju.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jfrqoqfe.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2reqesbyl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2fyfrnyfm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2wgdekswx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rniknydx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbwfjana.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2qpfcaeyf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fsaelrgh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xotdcjvd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gwglmqcg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2esseaeze.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qxykgtqc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2moccffbp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2czkdbzoa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2csudagvm.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2dzbricif.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dmvmevju.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bmodkclq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ggcekxsc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vydwalpn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2llfumvid.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ntnbzaoq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2httgwvro.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2khdmtild.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2wywaeael.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mggccqdc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qqvxnpci.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2deicfmcn.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rrirjauy.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2isvesuip.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zwnbchwn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2iolpkioz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2yzkqreue.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2kmfunggg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ltfgumiz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2hmubxnre.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2mgqvrflz.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xsecbzzc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2nqnyvtlm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2rslvzgjy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2teubhwmw.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ccrezhjy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2vuoaogal.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2jrtefsmd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2urtasozj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ohfeuhdc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fyzpkhks.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mkyhoycp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2myfaxknh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wqfponsj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2oxaoaeof.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2awawaltv.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2dbdaepjv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2gzeomluy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ozsqqkns.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2egdxtzzd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tugxitaz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2vryxqsjj.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ugxmqzfo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2asevmggi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jsltmlff.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2bvfxdaip.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vpkatvks.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2axjledkk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2frjpocot.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tgqorrsn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2uzfwknzf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hsldwami.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2noiaojvt.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2zjvwhkuk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2pkaicnuf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2tqcudsoc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tjlugxgi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nowpjaen.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2yeiirbgz.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2znzitaia.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2hbvxeceh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2obuwzzbs.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2imyzgfhn.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2fpgweinu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jzxxwibg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aueteqeq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gqoahchk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2vnzqhyjy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2idqvkozr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2gpldqfjs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gkbllvvq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2jekxjtqa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2iogwpdvx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2dzodhydk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ybzflwte.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2yakgauuc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wxyjbjln.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2epfzegeo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cyusqles.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2danmzenv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfpiatop.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2iddwrojp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqpgksxd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2vuypsvib.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2juzemvve.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2dosvhkrd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2odqqwrgl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uyddigzv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kodnplpk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2arqvoans.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2gfeemthw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fcczczse.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2exfzsoco.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xzhqvwoq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2usxxycxk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lxkgofcx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fqpfmtpj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lzgldkni.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2yfdzfack.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lqaacpvj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mnydwtpd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2hfzwivjg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2mgkkqzta.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2htljrzkg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ecvjdvmx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfkmeawk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjxcwfwz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hvbndqmu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2nuxqevcx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kdfqyypk.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rblsocad.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ywhlqzen.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbouduyj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbkjfauy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qfcdfbsh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2iyjjsvvh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2wilcddko.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xrkfhadu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2evavdgct.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2diiutpew.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2kfxppgtq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2yplejudk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hfxvxqjc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dibwjtxq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ebbojcky.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2fidqzwqv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2flsrpzwy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fekvmjcz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2yphqcucr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2chlreliu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfifaodf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckjvfzou.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ksxaqgnl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsgedogw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2yjkbzlzv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vlkguhxo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vmoqjtlq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2thkvmkfj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2olbmxeld.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2girdcoih.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fltvffto.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cxtpxmmu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdqqtyqs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2yfaasjms.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2uztlkpqm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjsikvzx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mweugqgs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dmdsfgdz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qxxuaswd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qppthiiy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zlhcrqob.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jawdahxu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2thsrjmkx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2bawxfptz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ickukcwu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qccvpybq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qjmypsxm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xtpetspn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ychrzvsv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cqyuxnhf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkkoddyr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2milgpqog.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2mmtffbko.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hxwvuipo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2smaqmlnz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fieslwbi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfpnfvdd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jopikrzl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2riaaonjj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2xgeagicr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2yrefwwgp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2yqcyhsnd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2tlwpzpxz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2yxxmffkv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vgqcryry.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xkgdbtcw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vzycxpzz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hnplhhcp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2rwiqrpza.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vmylzgxl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2fbhxttoj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vvsklltu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2byudjaty.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2dlrbthre.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2uwrzimgu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iyhmaswr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wyngaeik.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hggwhtqm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gvbfurts.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2plmcobuh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vphgdoyv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2uuyyogii.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zvkzuczb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qndwoicx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyoegwwl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbpqravr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2anlqbkqn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ocajjliy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ktycsyel.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2cheaffzs.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ezavesjs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2uejefnjq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2kaszccpv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mkgucwyd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gfymoqgn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2umyoyrak.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gtqgvhrt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxzasxel.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nwcgyycs.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2dtauootk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2pfodkjtj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ezsfnlgs.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2exqnppwj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ouaccjwr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xwllgavx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2plyvecgr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hpeyabzi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nndwvxmi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ohdpifhz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2mqdnvebe.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezketiia.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lmuzkpoy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2twffpigm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cguyabau.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2sutljwna.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ctxhaxsa.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ryxuysgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdoritpx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rnaagums.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjteffek.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yxbdptok.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lpsgbdti.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vykqfgbw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktavyvpn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kvmgxdna.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jchauhic.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2skpqhtzi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2uuakatka.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogotnvuo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vmubwroj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mzpdffoq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rlntopab.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bqcxabpw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqelydgx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vtrearwb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2kfwxxpkq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nmdixxhu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2bnqsnkzx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xsewysyq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2oyyzkblb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2oldzsgnt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2myywcfja.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dmfuqswf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mzlykhpk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zquoevsa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jxrnvtyp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gcxzvsgg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2axgztgrn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2qnjgxjba.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2idtupeet.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fbnmnvhy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gqdohvpt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2pzkteprf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2zhoydoyz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qxrrubmr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yimcymou.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xzajrmns.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dizgatpk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2pbgssojn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vrnsyyxi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jrhskkks.html


<!-- 参考信息 -->