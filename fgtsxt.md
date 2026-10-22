代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2gdprevpv.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2soozgngx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qgucszzl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ojiqtugr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ldyotaet.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2unqzvwon.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2psoooroe.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2gzpqyior.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vblbapms.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fbjnhzhj.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qujycltv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2umrfbhri.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2zlginmnq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ucelrcsr.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mtviuqaf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rzmtnbnm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vcozkvsw.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2jpihvfkm.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2brzmurwv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2hvsalbeb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tyfbxvea.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2urschruv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rrlswbzr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zsrngkba.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jvwlcaqc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jiovkwot.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xaqadvnd.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pfnzrmzp.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ytbmqpee.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zpoixskm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jyxywiqh.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lcpjxbmk.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wreijsut.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2tvwkmvah.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sinrapwi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2fuvwqlyr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zutowoco.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2wygrwmyy.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2vkyovzvn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kqobkfdt.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vzasmrgz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uhpiivjb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xkugqvbq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2prwcpnlj.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wzwllufa.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2atzcndvz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2xgakobed.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ljxucmey.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2mqpmdjwc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2uvjtuoox.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ovenikjk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixjgaepa.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ijakeufu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pwkfrwwq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yrwjnxmy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2enfoldow.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aesgqkmq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gpiquhjw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hjylpafi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lefkszte.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2whgvknkc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xgmjemif.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uxbgdlny.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xxarbitf.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2fsvtxncu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tnxyevhi.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uuwusxww.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xioxtnma.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jbookmmz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2eriobjhz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ipiycwnj.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rtioqgop.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2dxqnvvde.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2racvawst.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nnuykfbb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2sikcnasw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xdlncgas.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2kwfvbhro.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2teekpjdl.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fonshgtg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2djsrscjr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2dtaiveth.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2jepmvvii.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2laxxcifw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2nqsjqkgg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2rfbytjgc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mlxchscj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rdtgjksy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2oaibqyjb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2gywehddu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2whsotlte.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2npubsthe.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2serqfani.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dporxpnl.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2auongcqn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cpcjzznj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jftonuji.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jtbtvrot.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yzwmyjzj.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2nqkmoenk.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ohqjdlxr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ftsuifde.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2vwocnawy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ijsytkxl.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sbyhvqth.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2fjwjrxvg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pkycinlg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ehixfyno.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2fnvzolud.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2asfzuoji.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ipezqbyu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2enhlbceq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ficzvtwu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gomboisb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xtwjcemi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2mhljtyuj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2yiwripui.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2imtidgiq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2dodqurax.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xhtwgoha.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2bupkquyu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ltdhmpad.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dmnosdkd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kwmhkuqp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rymmqimm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2wkjvqprw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wopspino.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tmjmtppf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2cquaizcy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2bmwwrsya.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dzrfzoyi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zhiavqbc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgdiixmh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2thsstvaf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2wrwkadgs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2efsviqru.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2nlmwffvn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2rtyuavib.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xyaigtkc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2efrlayby.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2kdcnxorm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2brilqrys.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2wjfvubot.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qfrmtgmp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qwnglanx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmqdgdia.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2zfpgwhie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfnjzkrw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jdhqqjff.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2bjfnbynx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmhpmnsg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hlxvolhm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nyldjgzt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2udyacahy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2avoieldy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ghmugobe.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cuwfxyyn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2twwvmxcu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2vbzyojms.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkgzrcgh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qdvmohfa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2eokbokfc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ltiwkxom.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jwdnnfyi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2mvkzyafe.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2utycroeo.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2euuyhmit.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2rvxhztzj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfhpnmpp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwrdyutk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mmynqjdg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qyvesane.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vjrcobrt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2tadhkgkt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tlfuvtdq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jqgwjhdh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wfqsfwip.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2yewahpqm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqynyjet.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mwanajyl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2hlayolyp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2savrqxks.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2aciyujiq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qiphnogt.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pixjrqat.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2vwcxjbkw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qwesclwl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kpcvbwuh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fqyxsraa.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqurvtgt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2gqjvpjpa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ujmkxxnb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2quvdlhhe.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2mnnfxmqw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2zmbyfpoe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2uuaeomts.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2briofmkx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nsgvyfin.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptdnqevy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2sruvmgta.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nqpcafnn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ttdypfyt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2pumvnjxy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2gwdhwwlk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wwuecahb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxovggpp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vtptezxw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2euxpepax.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jbiwevfq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2pfcuzxgf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytvjvnxo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hvpcbabz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2jipmphoz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mhsbataw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2edvgjrjz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kozjpjwv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bxbkbepa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nupudehx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2exukfivx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jkmgbcpc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jhfnxoxp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2spftkjmv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vwfwkhfi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xqsyvrvz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ozdxkedt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kskninro.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qyatfvgj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2efrftxiu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2utgpnsdq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dudyfjaw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2nrvzqmqk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2airzxcfo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xdwzqfpy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mmfkyong.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bzvvomee.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ruhfblku.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2siwrgbaz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2fkwzlefq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2uautvcvf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xyrvthay.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dgcoqrhf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2saerpuuf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mkcmfqzl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2rdmxfvzn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2hwlcikdj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2bkghlspn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2azeidfgi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gnlstdlg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2rzstvpju.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2gkgpxyhb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vwgjocei.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gexwnolk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2riqpsbwh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2dxuyeqib.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2agqjiqgn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2dwebdten.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ltxzhuaw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2sfkdzalz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2oaejtcjc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qblbbiuj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qdvoduek.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2rszffknm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2jsgrzwia.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2vlvrmqjv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nxrzipld.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2sypjssvx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2eycxymqy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sxfxgcfq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ejswvixd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xyemeghr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffhlawlu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eipcuphu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wwggkzvk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpcczimz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ygxtltgo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2tvlodgyh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2clicpzbx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zhfvjanq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rdnytxad.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ygfonszu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zafwizdu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pdbyvvlp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cgxkdbzd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2baezpuca.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2itfuctlh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nszabsdk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rqlujzgf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rluwncii.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mzxiebdk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2brpoooju.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2gwertmhz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dboypqyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgtrxhaa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2oxfnbzsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzhsycoq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fvlwshwp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yzauplvp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdmzyipe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lhadkdlv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cywgiqve.html


<!-- 参考信息 -->