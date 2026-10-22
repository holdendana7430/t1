代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2vvpjilvs.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2fabxnnro.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2igzlqctv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mhjtsguk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pxsilkns.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ggenkkga.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lblxyzmc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gkzvqjvz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cilhwtwk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ndskuxky.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2jyadjncu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2znxhyuzw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2kojybqmg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xwccmzud.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2axikwnoh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2nuauumdi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sziumhed.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2jevsmzod.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2lhfzrfkn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ckaqetkg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nmkhxfus.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ttclulok.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hqugownu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2agxvrxmd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cikbyncq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rtjfuasd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eolmoxbc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kcwmgkus.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2cmdysnkk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2mstrlpqr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2aguubcxb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2syooibnd.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xenmfpmj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2nbhqdngp.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jmqpccyu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2tmfjfdql.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yrmscxrc.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tgaajngg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2mhmveqcn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2calsuhcs.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pieoutuc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rqonrbay.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2wzjlmayj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2vfxxhgod.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lwoqvmda.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wmkmicwi.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qdyjbvde.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2cfenyqso.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ueagigkp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2bapxqdin.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpqybcjn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2avybefhp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2tfvnihpw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2pyymlhhs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epnqgdvl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2mjqempnc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2comowmgz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dqzgpppx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oqixnyre.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jdesvgfb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iacghslu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jdkrvubv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iqetmfvw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tfsebutc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2rqsusior.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ginuvukp.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qasmpauf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2uzkcdups.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2skmzydda.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2hvocuoct.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2pdnijjhf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2vtpwplbs.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2mlaspelu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2bgnmshku.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2orvccgxt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ctpdbubt.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2kynuemfe.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rmrxtzql.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ruyriomm.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lxxkznxm.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hapfrbjb.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2wnuikkyn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ucmppggb.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2kkbevksm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2znbvoxbc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2zutlreie.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2bdakevjt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2gxxdjwfd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2cxpmmsyd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ypgkyepe.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2rufbtlve.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ktjlhmor.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2qscnlojp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gurdzhiw.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ykxuhhnv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ydpudwzf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lrkameoz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nvgiufca.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yaywgzhy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2fspsbgiw.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2szzjrxgx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ykrnmurp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2hssrwelz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2aptdkbnh.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ltbiishu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2kqorgwaq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ozegfxnk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dbxozvic.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bxydowlk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2eucdtvpn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2jmtdmekg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2utcskfrm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2upsipalv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tdlxylvv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yfasftmo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yojwjdkr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zcvefmga.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2weeedmxj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2zyiuwjjw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2etxiimpa.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2lqliazat.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2krbmrkad.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zmqusmix.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kzdobfru.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tueobaxy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2dnaimlkp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2khaybovo.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kqzsvhoa.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ariynxsn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2efednbvl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mstsrkgm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xrqurxqj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rcxjogmq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zzzfbppp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2dkcvkich.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sdsaswpt.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2aorqwksg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2wholgrvl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2uwggcxfu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2voaeqwjn.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ycwvqtbi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ywupydxj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hbreqjhv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2gcyxuawn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2padscmmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcqueijb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ayqkssrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdoqcswx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2zbzasuvk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2sqsyidib.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2octfvgpc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hkphrwag.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hjphcjss.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dusqyhqy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2qxkrlmyo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gkivuxeq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mwjxzckx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2gpyvdquk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2nvopmueq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2jjdrwwln.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mhfrlwsd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qvutczbn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tzlzdlps.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2pjziumey.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2nhhgmllx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fmawwmnj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ddkamgwp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2eumrvlfn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aezaxnkp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2isiqhbdw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhkfaewq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bcwnmkpg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2abatdnck.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2byopjmoc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fjykppno.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vjedfqgk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qzapsijn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugujnoho.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cghcyglf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pponhokq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2hcuoxdpe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2zdjzornx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2hqwvvbsk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnegtxyg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ghsxkpmi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ugwgncul.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqbtaewj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2veqqpfle.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bszixlpn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hnlhcqps.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zhetolgk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2larviwab.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdmmvwkj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2bqyktvzw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hdcmtkpd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xogciazc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qpiujmks.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ahbydacp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2bhzsoaml.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2wjghtnue.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2pqfzrkxq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2iierdhsy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vzkjwpcg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qhecugwf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vcuirctf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wzxqyaaq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mjocpyue.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nbgqrgax.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2nkwvbigz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2eebdtpnz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcmsecpl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2yryvcfie.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2kbccdkdh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qtqfzazj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2amzoxxho.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zwbqeqof.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jmdxnegk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ocsvehkb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2agyvwvyh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ebbsdhni.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2iqvwnree.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2taxpjhds.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ujmecfjh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lvgimdhd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkqdlrea.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2okmstqtr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wbrznnel.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hxarxmks.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iymzuztt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2btezxhhf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tmxzyfoc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2snajwkgu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2irpiigpt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ucwyncum.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbqlffii.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2opwlskkq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vumwqoew.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wwbnsjho.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2uijbfhuz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ybeozibo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2jcbrkcxd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dcznjoeo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tyhoujaq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qrrpjhbf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ouavaexg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rhpkjlve.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2sjwjzsda.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cvgjrcow.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hksecmkp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2sfrxwqhd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zxtwnbdr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2slbewjfi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ulymyjeo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2bvnbqjlv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2mnvhqgdb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dorldbkd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2maxahrbb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2adrmjgnn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2fsjpokts.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qmzimyew.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dltilymz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tnjxwsfj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2puknraqp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2rdwlikre.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2tsomumap.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2bmtmiqly.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2accvdogm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ppemrznz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfbmxmsc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2emqwnjjk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrllizdu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnbuyxqv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fvmuookr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ujzvscxt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ofilolcw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2gvxgzcal.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2fpjmxlst.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wrhdbvve.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hngmafrs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vwwbhcxp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xwkahpen.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ltfjavxr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cuobormd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bmlgstio.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ktrbnpmx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzglwrud.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hphugeuv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2avpqqmlm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bamxkwdq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2bksxbsuz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qjtzulnu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ldpaulon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdizcdkh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vuooxwyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljsjcxal.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xuizzscb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nworobtt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxzegqqe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncxperlv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbpgdwtv.html


<!-- 参考信息 -->