代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iarydjcp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jfqzlmvu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2patrncjg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2rglykumu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2boqyvwcu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2swtjhond.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2fqmhkuum.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2gffribpo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2onqugigr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xhcndqcy.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bvdilbgm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vfkzwgii.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2dwcfxpcn.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2xrwcewbr.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2iyggupwo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2pquzswph.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nodjwjbx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jnmqttcw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rkhwjhwq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ksvpkykq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tjkatqve.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ckyixnbv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aivigiyr.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gzhwrpzw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2zqppxsqs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2wsqaekjj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2shikddxc.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2luhleabe.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2modhzsrg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2rjqatzek.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2viasjsug.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2uciapevx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2papplnnq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xravghhi.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2auzeaekt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vxghskne.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2apcaayio.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xlklocgg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2flzeuyle.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ojkrqfxp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ebcdssnk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tapxjpgd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2invabdqs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2jsopmnkz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2zapoihjr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2cglerztd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdyrjdxm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmzqjcwy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2dkimbkxg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2yvsevjcg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2autojxml.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2hrhjbkpa.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jqmzhsqt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2azypogdi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2votzqusg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tjkajrmq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ksxxxtur.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pnrtogby.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2owavjlzj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hsxubqkj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2wlfpzvrq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tdiftawo.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2milbrqtl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ybsmgwlv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nzrgdvty.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2mqaeotpn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2pwonewul.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2qiavxwgv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ysvsdudh.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2vxnizjsm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2argstnzn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2crcfueve.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2vrttddup.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ajyakvcx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2fvxubped.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ppvximgy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mtopabrd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2bplqmmqw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2nqsbpyaj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2iwcztnoe.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2thdvjcoa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2fyeeskna.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2nmjpbkuo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2tsunsvrl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2daxnmbgo.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2qrwfqwvo.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2pcgspsvj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ezlpeddd.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ragnberb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hkfyyrlm.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2llffadzu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kpxfevoo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gzdpwtlh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vuiohgkf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2akqhqyqt.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2rrzuqmsj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qnyeprdv.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2nmlmidcm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2pmdnhiad.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2lplbzhjm.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cpnnrajk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lvmwgezd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2hoadaemt.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2quzdtcgs.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2imzkykbx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vcyjmirj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2zjovhghk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2cudwxzbq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wiedhsax.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ebqyzhna.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pnvokuqk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fhnhuhoo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gwlckmkm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2tpglwaop.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2iqydmbeo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2yxdjozmt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gubztcnl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2odzicqit.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qsfernwj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2lnpbhtxc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2jmomhzdt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ssflavdi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nreqkzkq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fatqliww.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2eipqznrl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2eurccnhq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ybuosyab.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qqrqfqht.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wjqbptsj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuezyazb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2orgzowgv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2jtuylqwz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ginxiaua.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2kcurdtcm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2jaqvehap.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2aglxycel.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2zzjfyepg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ibyjegyg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2nbjoqbuh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2raobwgrp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lmmuokks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgkdwlit.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2jtdfbkhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhfejask.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2wwezhdkr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2yltaxbif.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2setrqtud.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fynlxgqk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2swymozxz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fkehasom.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2wmhwvmtj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2qeofbaov.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cxxquiju.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qdkdvokl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ltqjzlie.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2flvlikrr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ztijqxpj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hwzirjea.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zqivkaoq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2yjzqagwj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2rmuqvncu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2frfvlnvu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2yiyfhgom.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2hfqywyja.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tpbbkkdx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2davnbkoh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yurqaffd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvtscdwj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rsvhppvt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wufhpggw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rbbttjid.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2omlqoauz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2cjgtzkze.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2evhkebue.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gkdypvia.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkczbgix.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2uapierxj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vcqlfnjr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2abtypovf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2rfishqca.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kebmlqsn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zrtiycty.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxmkdajd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrcnisij.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hsczucfj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hexpvohc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2twmeglsu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bvyperxr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2twxfwelt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2cgpsvrut.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2omiznqvm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ryjmoqdz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2axjiiyvj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kpqqqlwa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2klarwbyc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rfpqwwqs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2bqesiwma.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdvdofit.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2kyyiiwoh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hoqnmwhp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2jylnnkkq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qfafzsjq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hhpcgwmv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2janswldq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2dehoakjz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lrysmufz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2agyqjbrk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2fzsuvntu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ltnwrwhy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ybwueefo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rnergcsk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ldvepqli.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gnzirsfz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2oanekifu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jsdptvgm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ycsyqwdo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wgunxuoo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hygmnylb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2scbvdwax.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mcwxcweo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfoeaqqm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qxgdwhma.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kpzvfxfm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2fqmstdiz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iysmiyau.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2jkrgpwfx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ghyatpuk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsohocdr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ktsluiwk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2njhkeukq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmhbxgyw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2qfcobnhi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2glqjubtr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vqwvascu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2wtjrbegx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xwvipnfu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2haqvdben.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jbreqndz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2grvruroa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fvquhigx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2lapigokb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wpycpbqd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mdbzvhnw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cfsqdbcr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2lgwzyxyr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2rmjwtpht.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ejgdjczz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2syybzrmr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xgyusdxo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2yyctinuc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rvgzsfqi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vqtjrxub.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2fpcnkoja.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2pzeomloj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzfatcxf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ufmbdrwh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hkygzolo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qpimyfrt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2aaxlalzs.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2arzisyby.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2lkbsguot.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wffnfkol.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ecztdqjz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2jjojsxkj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgtpgrcz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bcyaoxps.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikfbxxxx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ymvmgnmc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2evmxipre.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2abfgnfxe.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ttslrais.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rhwrqwdg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2iyvpfhug.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mtftzgnc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lfhquzaz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zhilokwf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nqsxpjuh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zzojjkyn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gmmqvghi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gsxjmkbc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ezyhkwis.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2dvlagoer.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oznurlzt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pzosxflr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yxahxfwx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2caekmnvl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2lifawlsx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fdlcdnsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2antchrmr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jzyzwzfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkvqnfvb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2syiambnw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2unjtwgif.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nuplkhwz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dapjhdkg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nvzmoynm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eofdajnh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nloseipu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2azxuzpgb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2scdxzhrj.html


<!-- 参考信息 -->