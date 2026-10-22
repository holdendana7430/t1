代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nhfsochr.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bycoosmu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2wmgacxuu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2swdneinc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2xylceprh.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2fgmhnnyq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nqnevaby.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dgxuqhcs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xgrwjnpb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ovzngbea.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jxcrdozj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gmyiccou.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sbtmrpar.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zudljckb.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2awmwxalo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2qqnubwqu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2oiiuetkf.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2aqqqevio.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bhrqefjd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2teskhhfv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2bkrrbnyq.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2odjmdzah.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2wqftktye.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2bukivnrg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eppvmysn.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ehmzhwgg.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qkckrznx.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tpthjhvs.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vexigfqj.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tvfmuqsv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2emlsqsje.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2egrsxkjw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2yojiszrq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2fltslfma.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mroevpee.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dqmqyizj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jyystsgr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2vkcmuwoi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rkdhhiuh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2zmbvvjnf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ydrbntgz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2wjaxmpso.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2yvovtbgk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mtwduhsk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uvkiwetr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hxgqejkl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2yzkcirns.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2jdcynjez.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dglamphy.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nyrmwaef.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2tjdnjwoz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jeeglkby.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2shkuatqc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2vdgjhcth.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlnvzgzn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2wbauxwje.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ljwtfffp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xkiltjrq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmqdwwqn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2lammztrw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aflwsvve.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zvurlbms.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lpdnhlpr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mcfpenge.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2isgromwz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mjgoqtiy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hglimswk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hgjfeksj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ldfzfngg.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vzwosewq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2svdmwocq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ylmjiuge.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2whzykous.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2orolubuy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2emmgtaur.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2tirhdkyx.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2zxpmdbox.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2jfsqnane.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cjjrfrju.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2uplorpqe.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vgftuwho.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fdnttzsh.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mfuztyan.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2owhjmbic.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2sfmdywes.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2vhppccyx.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2yxhydrst.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ksejtlki.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2uithfwhn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2mfzjidlu.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wxszsnmn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2cbqzyncv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2pwtfbdbd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2rdlzhafc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2gwbagsbm.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2qeqaqkir.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2rpghuqfd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rrovbgly.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nfvvopmt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdfgtvl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mgizgeer.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nvugujgq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qwxytshp.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2bxdezbof.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ibzwkyia.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxxjpquq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2lpvgdxje.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2xlwvwfnr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2gnmttftp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ampdxldk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rinxtzgz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zqxjqaha.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2qakwgebl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yqkvckyr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vznmtawc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvgouveu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fvcnxyhl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fvtkpnin.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uouctdcb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hwrpvpeo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zhcyyuvx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wwiytapc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nowzugyp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2mfcztvil.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbaozczq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pokofilg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cphhhswj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2spofcwxy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2xlzdpzgz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2rubylzjq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zxsgmwhr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2sgssvgvq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2yccpjkww.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sqqoawja.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvcdephe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qdstrapp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2lsblxypl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cuimhbck.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2svptcmth.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pojtfczb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ytcczsfm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2xfheckwi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2rxcifkxl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2cmshnuoo.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2fkkjpkxu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kmzekgmj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2fyeuxidt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rejdoitu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zqcyruwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jyngjtqd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2wfnmtwku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljqhqufb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2gdkqzlcy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2otpvshbv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2eaqakbtt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zsfgrrcq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yptufdjc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2eqdkvjdu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2scopzppn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2waedliob.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2htkcfasb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2bnrtxdhi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xiuknxgg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzwodxfm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rxduxtfe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rdiakevz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fczdmejc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2sscqmusv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ulsyxuju.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jtlqbasb.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2nxzlanip.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2bcboomom.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2syhhjvph.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2injaupqb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edefahhk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yrxvvrqq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qqqmhkvd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2adtydxpw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xetrlrgx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bjazmxsg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hwqmnyiy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2lcbpszpj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2srpkgzyt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tixunjxm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xiiotcig.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2lvphvvdx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2cotgrfci.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2nnbphqsb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ywjerwkq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2nppayexv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wduvtzuo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2aszglncf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxsntahi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gstaaicv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2whqhavme.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2lvjjvfho.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ugkfjsnk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2onxspjhd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2oexvbrvd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyrjafox.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ykhxupvn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2yniqkwhf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhieiyak.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rrxduihn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2gjxtkyhy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vqqirben.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nyqbtjda.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xgcaqmfw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2bveawngm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bgwffbol.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fubmcgsh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ciaxjpjk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fofsglsy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2azinpgea.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iomxyanc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zadefzkz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ordmxaut.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oinwgrbr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wjhctkho.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ngrombti.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yesudkmm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zngybxrr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ylwsfyxv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vzzeonjx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2abcyczob.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hvcxpugv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2temjebyq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jpyddvtq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgtgfblm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wmhtzjuj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fncsroux.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2bsqsfpfa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlhvypxp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2licxaopi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mcuvaezz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rsdzljmz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2yuhyfdha.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jfzkowdq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2krulhaiw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ytdbedmb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pmgziphs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2zqsukhlw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2fsfhjoww.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2hhdmxgof.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iedhsvca.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vsihoych.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2syasdvaw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2uctrqzar.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vmqjnqxc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2pzruaspe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2yrmfmgjx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wyxjvuxj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ntsgkfwp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2noyepjvx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2enjmcobs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yxqqihvb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jmzcowal.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2plpawvef.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ojezmjfo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2nsmhcprc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2unwtdmrs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rakxtpgf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnzjpnfd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwuufmwe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dpkkxvqe.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2pugqhiro.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2sraebouj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fyxssiae.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2fszmtkab.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xqaultsr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zgveakal.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2dsvtesmv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ptlfcigl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmqqdlwu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2skwvmqvw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bphsatjf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mzxemvri.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rkkyqpgs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ptrornum.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2usbfjysq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2phwoppet.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ddmhpilc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ilvolqsi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wxokeihd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2adphioiz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2clenjfxn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xycvkxcg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bgsacsiu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2hrlhgvis.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jarbnacs.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kycgrwae.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fnieuwjv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bnislncu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kcpvzqiv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2kmkwxpry.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dzdvfyel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqpjjlml.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2zvtjmthc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cpgpqgnm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yhoebrxn.html


<!-- 参考信息 -->