代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2snnsrfln.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2apudtwja.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2arvxllqh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ytrhduqv.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ipooojni.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2zcrzqgxn.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2hsyhahkm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gkodhfjm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wxigxfqz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2feeyayoj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2rhjhvswd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ywjjarye.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2yotsmnzf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ncqhmgvj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2sjfintet.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hmdhkqnl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2baqwmhsx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2eaptzvar.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wmlyrmdd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2eosbhqic.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xpcvtvxn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2taxhoauz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mcmqppyb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2boxhurjj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ietyitac.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lnytivic.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2qaqtvbrh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ybpbbmsd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tzhwevaf.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jemwckxm.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2gapkilsd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2mbymltol.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kyqshjnt.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zhuztfiw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gnksdcxd.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pulnuuni.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xyvqrmol.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rispvbcr.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ppxixzti.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cmpdbuty.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2bzoxuloa.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2jihoyvwm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wqbpoodf.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sqlucqjy.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2unoswiiw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2luvrallg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tngwymzv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2jgqteane.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gfcwkrdg.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wyadwlyg.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ccpmdxts.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mlypmdww.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2knvnkoct.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cudtzsul.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2nnazqarj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2qyyahkmk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ehmlspmz.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fzbohqys.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2cbocexxy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2vrdenawn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2bvojspzz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ffnzocxf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fghrnoxy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2bjektcdx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ylnsgnnn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2xgrgxzba.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ttpoayoa.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2wdeolwrz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ebzhlwof.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fbxiguqu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2doclozyo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2emiyktay.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ixsykmgr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wigxyzqw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ysznzwfk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pyrbqkba.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2zamwoasy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2knaqpffo.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xvfiuxlw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2sailgmne.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2otktqvyx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2fmekwndl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2zrkbesml.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ixszjbnt.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2tkgvycvw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2pfbakocl.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2suimppgd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2pggctyuu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2uydqnofz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2esvwbmfq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2lccubaby.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hhcpajya.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hgznxelr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2rfewmrln.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2fmmofmfg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2zamypdkr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2dhmrdgnk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2zridkahs.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2qbkyrggs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2jupwbswe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2yibkcucu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2cfmsboml.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2cqjqeltp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2rtxvqlnm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2kpbejcbl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mtebjhvj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjatsrmi.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2sputqzmz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yjhukbzj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zqosnmsd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mtvhfoyd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2drqptvnh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2isdlnyni.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2asfhmnpv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ncwdhcst.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ikstvcbv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uxooehwi.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2zajdmpsr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fuykzetd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aohbnvdh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fgqkvogy.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ncqgdcip.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2crokjvee.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2oonokkwn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uytsdmzk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gsdfgpwu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tbzihjbl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2igvzyztv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ggndtbea.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2qeypfwgc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2nbtdtmvu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2yvkpyvmd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ipyrcvxx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hunmdeug.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2aabnhpjw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2sbohzcuu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2weaiytcp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2anhyuqga.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ziqrardk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vcctflqe.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2wphqbmzq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lsoeswev.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jyypqslm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqyfhhfv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2rivpvmac.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cqbllxto.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2bycgphpr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gxtiariq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2yzejrejr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2hrygzbal.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2nzqhytge.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2igbqkjuw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2bzlyookg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2fjytyqen.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2suvxisrj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2jqfqltnu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2uzbruonq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbyuxhnk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hkfpyore.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdsztzlv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2leiooxtd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2gdmdktir.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwhdrsbr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cemosydv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rvnrchfq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gslttmlf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zmqwhgly.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2siwdzwoe.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cfztllct.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2szmcibuw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2dureaysl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfyngfhj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fzrqhtyf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wuhtsggo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2odkbksqs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2owacyosz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2brkhugzl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pinskymp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ghlecjxi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ravzzpim.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyggyaze.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksfqmzol.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dkwgydtv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nvryscbv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2baqlbwuh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2mlqngnfe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hdinvpze.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2acladwsp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zbrpvnku.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyazjuqo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bgvkyvjr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gmssvzfi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzfgkdqf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2saeylsxq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2rjmimheu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2yrxuzubp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xzcnptis.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2eyichxhs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pwtvvjad.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdbfvkrv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kohwaaff.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2twithjqs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2dflprkju.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xgbwwkqj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2uvdxvwme.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2yktrpdku.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2tspgkhww.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2wbygnwrz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqfjazqk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tsqspgvc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mupmhvlq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2bzvsidua.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2cnpqitav.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtzqaeye.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2pmfiejnz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2bszbgwcp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2mdwdjaqr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpvijjuz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jxdxvmvd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzuzzjal.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2vqdgenjk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2edlpcyfy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgqbendh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2sqgdxumt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2oydoisii.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nsjgjjrf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rvioslnu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2atyoykyz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vgimccxi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rdtbbsjl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dbkqjrxo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2aywutkqi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2rwzwgugw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hweagval.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fguubqdp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oabcqqgk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iebpzpfx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdfferfo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uwhcxxde.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2zjsxwuzi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytyblqzm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2krgovjvq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2qqoxbiqx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2viwtasas.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ptjjiqqt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dimoyjuc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2axazxbum.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2agdmpblh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yrgwfcpa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2voryvhgc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hfqpgrfa.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2pzymbvpt.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cbgxvqeh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lgudpjsi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2iqhuxuue.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2msswdxtt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2qxshsszr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2juvjoxlo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2kqzcsuqe.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lmicpxab.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2cxzbkzho.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kzquuxvb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lgvnnbpw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nsdtqqup.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kxscxjsb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qgqraanc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ruofhvad.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2nfocsrfw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mjemhwbd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2uzfffgrg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ioyotcsc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ohtnpylg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hljuiirg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2paqtacij.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2agbqdpjp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2eamfbzxo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2cdynpkao.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2umusxelw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ynnjthzg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ydhiqefs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2euknsker.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kusarirg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gtwcdsny.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2kqporzuh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bpqvmbbo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mrqhjzto.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qjedklza.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2fpcpxuzs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fprnvkaj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2niqjcsoq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zrncpbgd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2falcsgxj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oazlmffc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pcnileeh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lmdkcdpg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2plsdnzdd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2yecicyhn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxkvsizi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2omsofkcp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qhafuhel.html


<!-- 参考信息 -->