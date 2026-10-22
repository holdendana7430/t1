代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qaaehavv.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2wkqzybhz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2dfmmezlc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2onjtejuk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gylmwvfg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bovqmvmz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iwiayljs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2okwuvxyb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jcrwirti.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yswutxvw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zfuijhte.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2lyuojfse.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2owvwhzij.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2inipcsjy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ujtalntc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2upybmlyu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2eufsxqst.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gcipugyd.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2cghsggip.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2bbphxmyu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ryjjxdsz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2suqibkbd.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hqgeemcl.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xvwvtrng.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kcvuixvt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bmvrzumj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2peoaxugs.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kzlshhny.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2fwtbwbey.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2xrjphrld.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uwsjduik.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dmduvuaf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2slfgvllt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2glkkevzo.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bneqschv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ofanepza.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cetprdnt.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uisiqpft.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zrpuzjwv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vajmrhkr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2idhkksqc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qldgiyuk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2vfjlycbw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2knozvdow.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2smummlky.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ocgzqzzu.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ktaxqfuh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fhusdqua.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2txpmjwav.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2qxaqmvjp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bduypqru.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ajkwyhwc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2wyevoboc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2qsuxeafv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2habczwsf.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2elaawxfa.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lggueelx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rnofwweh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fjolcxgx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jmgydzhi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gbqdwtnm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iatroaan.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xsqfhmfu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jhuuhicp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2qxakthhd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2lbrbwsvb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2qpfptvya.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lelhknhl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2thfqebwo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2pxkvajuw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2wvualkhz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2xbcnjzrj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2glhmvaud.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2munjmkmo.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ieruqcxa.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ixegqpmf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dteunfbi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bkodbmid.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mnxqntqk.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mkbyyqlx.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xgxkhcob.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2frscfsmm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ejwxxnvn.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2htjrsqmj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2wirngvdv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2apadoawi.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2dyxzcpnz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vbjvzhps.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2glzkeidf.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2awxuekzk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2itkljfwl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2yfpcsqvl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2bckraycu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tqajayfq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2icwlwklt.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mlybnboj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vodnlrbp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xqwapaoa.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ibwqbjon.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2oapfruzx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cxekzbdf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywmdvjge.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2sdswkrma.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ejhqpojn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2arefldex.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2nhogtlyp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2bcxayfhi.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qminiiio.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2hfbantgy.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ydzuiqhl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2srrlksvh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2vbfuhdfr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bxehgvzx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ixxqtohr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2myvedxsk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2brnsnmyw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zhxqbdwa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jflfawif.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2dxujrfbf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2jhuuljqz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2evwlimfc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2seaoeqnh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2oirwwzuw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ezclimmk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2xwotfclb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2rbiiepck.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qstdlmdp.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cmwbhhwl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dpklfsfl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2aymzmygf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rgyqiiqt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gxezklrs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jsuzuyly.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gualuewm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2pkziybwc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zcaelylf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2vxcomyuj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2llcmsdum.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2goflquqt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2zqxhpwdq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2julmbtbk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zsliawgr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2rjvxtqqi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2uvtphsbt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ulcvdbkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehubxytr.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2uttlfqdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvzqluaz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qdnfenkx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2msoieudf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ckkpktct.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zturvfmw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wiptscyb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ifhgsvgo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2pmywppce.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wngtrghu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vpnztnfi.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2uatrjcpj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2pddhnaiz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxpvxigr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lgwgftwc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2madoscyw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wryiduww.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2bdolyiwb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ozidsaoh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kacwubpl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ymcgrsyb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ndasgluf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jsmbwuwg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bclpijxm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ryyevvhw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpvduwfe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2outfmchc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ialmxulp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2znqqolzm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2plivarkd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2tenfhble.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhobosot.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2skrcorip.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezfldpvl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2edmhkrip.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dtyltoqb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2zlbmzsul.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bsntytca.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tjuivqmn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2sysgkgfg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ivcvsbxv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rrpqesal.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivmrohic.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2whnoolcm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2cbnscjet.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2oyfcwiup.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2kmtnbcea.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2excbwndz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2agqrspsu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rprvzepk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fredplcq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxobxtxl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2yntdoubc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2kbthleyq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2zerspgbz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2znndwjeb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2tfxqqvbn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2tnjqtdew.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydpmzpqw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kshzgisn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yvcwrevn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2oqejdbfg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jmpwcjtz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2wqqqawmk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bxxtvbri.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2unidtdrt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2xqdvvxsc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uyvjbyek.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mavxmwuc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2croqfjru.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nfigrlxc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2joyilqtw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2okovwjqw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rvpvbzwl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2fpmgzaxb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2frirayea.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uigzrrjr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqiqeion.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2poduesid.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtrzsxff.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jamliflx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pejrenfv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rgtedyho.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cccsgwtv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2vtiyelcn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eosigzrq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mkwjpdyy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2odnwgkdv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2awzfuyvy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2sxchiiqu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rqjbulen.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ousocvcf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zculbfao.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ysulyifr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2krtbbadw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pzonwljb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2imhxelpq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ebyowklb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rnfcxigp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2opezdmyb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2najoefte.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ggqulwod.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2zrclhivk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2hshozzcc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iretvcdr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yptmznxi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2snqcbnye.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vaqzpnjb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2jtfzdhes.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2plzjsvir.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nxtjglyv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2sunqnchd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2msrkddja.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2djgciibs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hkozoqzb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2eoifmfgx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2cmfijgyp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qqkcplfp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2bgaldkvs.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zjpxjpmm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jwsycdyu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gcnowmnx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bkohwcki.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lggssfqf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cyektbth.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2fiwcsvcr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2svqldvbt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uwwifcdc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hkomtfth.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2gvvttvkk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hgfrinlc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dpddfxho.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tqqrcecq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tvtroouo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2najrkxnl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lwuymnar.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dkomwbxd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lwkraexi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kdxlthtw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2sbkfgudq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fugvruot.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dorruwcs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2esdmobth.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dheqwqqx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rydsmsrg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ephcuzcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvjokdru.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2efyofldt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwbnrypa.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhosaxoq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wfxobopc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujemeoys.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2akjxbndi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfyzkzea.html


<!-- 参考信息 -->