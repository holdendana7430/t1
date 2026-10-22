代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2wbfdtete.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2mdpfmqmh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2zqylebhk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gssiazgk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fyvaeocf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iwzwgznt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mrdbbsgt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2xrrgsnxy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mlkgmzqm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eeawnsmd.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ccarvsqu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2svcuknni.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2epfjlsmu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ovbhatgo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2swpljomd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pllmrlwo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gwxqsnzc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hwawaxxf.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2mwqkfmtp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2euctmolw.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xkqyopup.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yqsncgxq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xhnhqyon.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dhtlylsc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yjnsmmjp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vbheklol.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ogcsndcj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sytnlztw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2jxfnmpvp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2czrmabbe.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uahgqfme.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eznykvrs.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gjssmitq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2zfnzghis.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zlkjksov.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2gsixckin.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2noojzpfq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2pynsltgy.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2apjdgbjt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ruburhjb.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jmgubnbp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ljcchmfa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2igxwunwm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ruhiaoat.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2omehxklu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lcrysatt.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2haowpyho.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dkxkhkjm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cpvpigne.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2womumbhi.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mihljakw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bldwdhft.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2dydzqtbn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tqctgivx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nmixxsga.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2hzxytcca.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qmttkucs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dxxowzxo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kouahufp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zlobyktc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aqhimrrd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xjgzdwkp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pgikzqgb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jkcdkjqh.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2kueckryj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2yqoolqeq.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2aaicymed.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2eqdmanfl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wdwtzbgl.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2njxmjbce.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2yfgwcnhq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2hqzvfhaq.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2povivpkm.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2lunsobmo.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vobzkgom.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2eosxapuq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2qowemlok.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vzwchaet.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2hijrroki.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ehgtlamo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hiturtln.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2xbiisirt.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2cqtphbcy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2kisnihbc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2atldlgfi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2wyjklgjs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2coyyqpzc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ipnweqdo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ixzuaxjc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2mltrhhli.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2tdjfrkew.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2progblic.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2qhhmlyyp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2butzdicd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xcdjvpgh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyqrtrdx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rkypstej.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vdacpzde.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tihnhzrd.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2spwumjhq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oanzhhzb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zjgvtcyf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2jjnwnosz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2zmslzgcf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2dwthdyuk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sgnxnttv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vraiekka.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2gftabjwq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kgkalkst.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jaejngxb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2vsglyreg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcpmtfig.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2sicbwtzi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2giloyehg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2njguogvs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aekfpqsi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2drthzhnn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2icvhirlo.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2tzxkekyh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2zvkatszp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ahezdrhz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cyufobiz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2subnmcxy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2inzrrxrp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2fnyqjhjz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2rphaegva.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jahnnibb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ifqldfwr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2asyxsizb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ygigkhgg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qekaclig.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfzfmsoq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ploaawyj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pispezvu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2injzrxpz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ijdxhdit.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2yxanredu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2flyoilsd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2kqckqvua.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2dhbvhqmw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qodaypki.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2sotutglf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2qzzlmlin.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2zgkcifaj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ojitumtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2euhtwezb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2nfkcfrum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tdtdabhl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2bsmrozkz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2xpjreqrl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2scwcvgja.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gnpgxgpy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vjqcgcri.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vuxpllig.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2tbuuluks.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2xdfelkjt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kgcvaqwt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2yvzhubfc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2twiqbfsx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eofkeixk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dhautuzi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zxetahgm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wzsqoyna.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2duacerih.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2yllgwnke.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dfnbtenc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2edxssgto.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2aqcucyuz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jlracuvr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iisofacq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihggjepw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2letdwofb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2esoelymg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2nazeknab.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dnyeopns.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dicvcwao.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rchhcrgj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2sviqgocu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2maprvtew.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gvgslfsz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2onzdvomv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2utubwuis.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2vsatqouy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qffllrxm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yiutcwoy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2nssgweym.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2yhvjqtok.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2resatxek.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnwgagji.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzfjqjya.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2jdftzyth.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2cpfbefoa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnfkumdj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ayqiruyk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qsbcjkbj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2arpcxtfz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ekjckfnv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zkpsyvxd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2caouhyaw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yeyrzsar.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fuxjszsu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpbmlkff.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nqymlvek.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ursnajxe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnoibkwu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2djofqfxd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xobipthu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2diogxfkv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2vputmlml.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2cjlpkybi.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tfnomwnu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2flswdhqd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dbmnproe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cezufjtt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nmnctixg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mmkbnafk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fzkguoqk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2esglyndf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vagagzje.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xuqibkjd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ibbhbfcm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2oovcorrz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpqeltwh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mthhqifx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2phdmhhto.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ycnzuujr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vwosafka.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2pzkentbq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xlgesitj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2eruzrpwa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2vlacubbl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2gwfcrclq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2eprzefmg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2omgczerd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2udwczgur.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fxmljnwn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2pajppjnc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2crhjpqhu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2sptneupi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xnjvbaqe.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ovazofjt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2chuklluw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2uedpjwjo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gtlbkzob.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2hlbzeeaf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2iyexiekp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2wroyabvk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2rktuicnu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jkqvdewb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2bmdrqcyw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jkfqnxqx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qcezrapo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2moirngrg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2pmuemona.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qcihnwfp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2qsxuqblx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ehugnlls.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2lmzzrafq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqbojbxe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2byixhzki.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mzcyktyg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2smrgjqil.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2qtzxrwkc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ijanaqpm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vwcycmga.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qxptwlio.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qudycmub.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ahzqtiip.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2edrjelmr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xublshdp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ltdieemg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bamcwbhf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ytmbgckt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2piqsddfc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zndclzuj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ajhhhlby.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2utywgllq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hacsiryu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gqjwvbwp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2irvrgcxf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cnnadxie.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qzjqsrfq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ysywhthn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ikqzrqip.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vvwtmwnw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2yghzgenh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mlfrgfyn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lztorveu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2shlorqdg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vtdtdhok.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2cbodrlob.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qfeigpkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnzyyqiz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2zuinlwxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyzrqhtg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2elkobxzv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2hufxcrio.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkkelrqg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kinktlzm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylzekzzw.html


<!-- 参考信息 -->