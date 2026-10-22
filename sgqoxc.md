代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2grlkiowd.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rglznefw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2vxampolt.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2zfcpyhyq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ugyjarum.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2hjmuezyt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ivdaaqyg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yeitorzj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tnjrxsow.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yvlljmqs.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ebivahbn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2cyyprnqc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nvndskvn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2igcnhhom.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2rrsmmbzn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2wsvyfqdh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2donyluaq.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2pgnvnxun.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2khdehfek.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2hcqfymcv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ewlszqox.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jmdbicfi.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2lpeeekto.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2nngxpbgb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kiybsfll.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nvazrsbv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jtmfueui.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kpdzmncv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kyoxevoa.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mwnwomav.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2laqyaqxy.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2srnxbpho.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2msueepxd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2disdrktx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qczirhqg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2plfbszcx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dljhmifn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2nsshvctf.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nccfiodr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2pistgckk.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rafdrfat.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2eawqevtc.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rudzxdok.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ocdbigjd.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ptybnyyo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2slytxdie.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2jkdraqfz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2yijfypjl.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lpaalqdd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sfifbljh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2nbcqxzzx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lckmqkzd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2zbmebsar.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2uhpdvaaa.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfbudnbv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ovpuozyb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2zwhzcwtj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2htbxfumh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tltzubli.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2rqdspjjw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ttnolxor.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ihhdhqqg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ugmzlqfu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cpxwdtlv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fpypcjuz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lfkhptps.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wseenltu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rnnifuhh.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2vvyqkwuk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2szwhkznf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wpmhunnq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2devsilge.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wbcqrrgj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2obqvsmnx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2oymvotik.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ppwusfew.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2cxsmemwb.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2uwmqhpyv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2cwbvizdl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2gqhgrqwx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nhfuiahj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vgtbsmyy.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2xqqyxzbe.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mfdusnpy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2yguzkdhv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2awdghnpu.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2xkglpfsq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2zmzsemtq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ajankquh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2tshhrsjv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ctxgtdjo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rfscarmw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2lnafokoz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2obtcpukr.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2udivknjt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2pzehkris.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2jwmugnjh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ilhcvcxf.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jfggrtga.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fmzqfatz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2eguqaaap.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rjaswlac.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gpmqgybi.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2llpdxosq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mqnksfqp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tlytqvtg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2riwarpqm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2gbfhmpzq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hhcpocjj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2zhdrdwom.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2htmmzmhk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mjzekmbd.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cmektdlf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vyuanhuo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2erlhepzb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pkyamyde.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ytdowemf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jfqmzshh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nxxqpgii.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rffgrign.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xjdfzswm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2bynxmlmd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2jtebuiqp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ofwdtsir.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2vyabbngi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2blaorraw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2evighhmj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ndwemzse.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bpskdaag.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2qtkenggv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ucotyrgn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2acpwzgws.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2buiexapa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2migdovup.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mhezfgkk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsnyltdp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kcumbupr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hovqanha.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2rmthxoqd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ygxnhezg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nlaryqko.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ixzwjjeg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2bemogljd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2kyjreaxw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2uojdaeba.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cxtdgriw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2iehzoeej.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2urroeezm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2unuriizf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngyxwcod.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2gvmhjzte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zeaqjmnj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2hoyrzfpo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2trwizmic.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ddhdbnws.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vivjflvl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mrdhqpds.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dzaejpad.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2tetibzhe.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ueegdfne.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ombmkyiv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2lhvpjvnw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2qoeajpuc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ckyxqshg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rlfvasaq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lmimmbrf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nqbxjowr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2qpbubxci.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2kjtncyqa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aqgaiwka.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ttegiicq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tltlljbr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cahvdavj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjvxngzz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlkafgcn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkvvbxmw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mbwpbbym.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hiaxxdcu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wyttaavv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xcjxpoai.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xewulxtc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2sctyzztr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mklhubib.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nvmdykck.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lssbhhdi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2wpyfbrpy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2cehxbyir.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2rkqrqhye.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2byjwhyng.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qdcfatzb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lwbjrksr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zvwhjnpp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dvhawfjx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qoircnib.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zettzbvn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2nwsflfht.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2yrgfokca.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ahnuchxh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2vrpytejr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2uhhzwvkn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntsrapby.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkacavpt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2cvhpnijb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2kwkbqnsw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ojxpywwh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rzzbnwui.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rcunwpoq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkkurtkp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2udkwdpyh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wocnbuwt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xtgmjjwd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cayfgdgs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2oosrnpav.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfglgwdn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xdqlbcdc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2oxpqodch.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2dobtficz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dafdncjk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rdtipysv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pclbyohq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iggeudct.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xlwmfgox.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2nitjwggc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2askbggmx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2dgfzjboa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2bwitwtug.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2blclmxtq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dtjsfmyz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aisfoubr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pcxzpbux.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2auyrrbau.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2jserjown.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsrievnp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2unbnflcl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gvijydxg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkiymefz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ntfhfmmc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ffklmojx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcnwvstj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jymutoey.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ltmxsrqp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2zzqpfacv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gtiflkrz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2wsjmohno.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yhdobyon.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fzeetasl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bjnrftod.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mrhcmkdw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2srhftvol.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2vgopgpac.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hlhnuzhd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2guarbgtj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ldcerzmq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2bbpjwakw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2muspnsvn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fmxmnpuj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kvvusswv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2lfeiuhzt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xvqnzhlf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ckbqmhdl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2vxrouvih.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2flbivtiz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxtynmkp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lknruieq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hhstwuod.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mifhyzvx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2pvqktbhl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gjqvcklm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2aozutouz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2vlpcaety.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2grwichew.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2niaqxirx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yapcioqk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hnyckjny.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rmzobewf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nayaslik.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pehvnlqn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykzravvm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2sgbbzeec.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2yqzhpczp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2qmxvrykj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hiibtixj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2relaltxv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2msvmvsdh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fuqyjdti.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hibqpbwf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ygiptkkl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bbfdkvxi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2nlxhapjd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2skiigpoh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gumirvfy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vuoyqhve.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vqukfrqm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uvawwuwy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2zmbqqgmh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vbvclpmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zozrfljd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2tqowowum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzjhsxao.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gjmnjvxl.html


<!-- 参考信息 -->