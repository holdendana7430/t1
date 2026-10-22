代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ynfapnph.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xuafaneu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2aqhedolt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2zvmjxlez.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2krnwxfje.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pgngqbze.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2lftlxkbg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2tackvghe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2gbdmadke.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gkutkqfj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xfrlnbwc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xlxzqywf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rcwoesvx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wvimzcsr.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2acovbdrx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ysupbgse.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fmgkibsg.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ocsmgehq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gedbjrqd.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2skcpvzgl.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jwanqaui.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2daaxozxu.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tnjlawaj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wxlsbras.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2icsldakr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2qcbwdbmq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qslhzfts.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2frbdayku.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2febvcifx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2gvsxflpk.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rlbealue.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2wofbczsb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mfftvhmi.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cgtcgoaj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2hkkaxbpz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mcgpibcf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xphtuara.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2luhcmwlj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2wnnarluf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2uxyvnfgy.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2itultedk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uvbaovvg.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2jffhozny.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2rwecqgfx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2zhmjughs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ektwafbw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2pxtzqrcz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twlmekkg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2znvbqetn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zlznzbpu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gihjkqlh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2fjuiraiz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zpggafbo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wezyssgs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ipxsjsor.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eckejhgj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hlabdpsr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2urvleryt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2glhjqbhj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rlirejin.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2roladwow.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2iosgtooo.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zqupaoud.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pxdmrncb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nkurebcl.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2cpjololt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2uzrwcuqd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2pczepsan.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2mvydmaer.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2piohyxmo.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2buawrnvr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2evfbcxyj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lmoyftlk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2smcxplbw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2qbejscdt.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qqesguah.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hesmvswf.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ytarqkpy.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2zuuythno.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2sxsklntk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2nktmgwud.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2mvekcaxd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2xfjgqzyr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2axvepxit.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2rihglzbx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2hhhnlvfy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2eetriwjt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2mnazhtvs.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2weqfszkz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2eoqyibhn.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyzqltfy.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nynwhxmr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2aqvksjnc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2svbaltid.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nkvwsfyl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2iljmtflc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2eywuqrjx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2awotimmm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2mrqpggkd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2akycuzil.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2htyksrmp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2catwpoyi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lvznscpl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kkwkwdul.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xpalqnkw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yxvolnlw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2djlvwkyz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2aunmntld.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jemwpube.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zqnecadk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tnikhfou.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2cepzorxi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bzxhfzbo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2pwhkqnod.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2uvdeblva.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2rilwtwdy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ddptxxxj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qgbrvabk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2estnwsny.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2zleqxcer.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uypdecjj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2pqeneave.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dgcekmcj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2domourhc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zpggaxxc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kbxvtkvv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bgydgizw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2opohanru.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wfclokln.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2letntplj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2kniwvnwo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zojcoekv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2zdfbwyeb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2oyprpcqx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2sfqxuudg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2pedqlzix.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2vhrwyqhb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kjgurnrc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2dwjpeoqf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cbfpiwbz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2dhjwuuvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clvqfhic.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lxgvftkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkcozkfp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2nesxevlc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pytosokx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2lyvlmqwr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2opmjuxim.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ddavubnb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fxkltoao.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2gwlxsamg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2youudnnt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qvwqenqh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2mnznzadm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2lkobljsw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2azcwvsks.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dpgdwubb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eqwblwqw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ledalkle.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2zlwabaki.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2pflhuffr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hdlzyyrx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2uhyzjrtx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2iuhrsqvv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2axzmriez.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mccrqxoc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bndrecmw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfjlvrrt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gfgmsyvl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2nxovtqwq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mvmiemqx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qysssgni.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2uibhymwm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2tsnwgzcf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2oizviubx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxfipbtc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyoojewo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2pxhithfy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2eusbabjl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ojhpgpwj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bikshzmn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hntwzshh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2jvufsodv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2swlmbnrx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfvjhzqc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oyazgohc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ttrtghnv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2bnksqtar.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2tewaeypx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2aozogcqy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2smimqrmk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jujnhily.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxsysrfh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfdzkhul.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkzyuqpr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2mdhjfzvn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ixcpjvrm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uawnrgnz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2qxcsnard.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2gfnfetvm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rqubwlwo.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2imaobaou.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kwkxdxxr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pnqryhov.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hzyplnpq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2hskewtax.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wzjiabpk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2cgokbtyu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zhfmdzdd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uemzzubf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iwsvsjog.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2icummkzr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rcnzatxw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bwopiwkg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2bcyzxqxg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2puowaoky.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mwsefhyo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2bgdftmoq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iypkzief.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pkjwkbch.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jjifrwya.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vgzkjyep.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2izyhxzpv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2beioewgp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dqiixybq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2txuyemwo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2abxwfsyk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gegnhxde.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kzqcpzjg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wjwrrknl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqpcuxal.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2zcruwihg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2irhwmvdy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyfkcafq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2fupcivih.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2haiylwos.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2kalduufp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2epbpurtz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fcfmchps.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pxklvaul.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2srycnynw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nfeqesus.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zblrqpdl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2hgdtpozz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2nmimkulf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2prqrrito.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jojkxiiv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dyobavhw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bltrljkn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2owsaublu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2knuiahby.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2esmeoybv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dmspfizh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2yceepfju.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xpenwfua.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oybleorv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2edmqwtoh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dtsldyfs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2kojcpiyu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ycmuhuqm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hqivjxlv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gicgceka.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xojrhazu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2bfaeipnm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2spwcjkua.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2plsfryne.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lefsxtfz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdcywgpu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mtauzzjz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zuulicpx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jzpyxvzs.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2sujqyltx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2bxrndnci.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2inkmjxbt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dyslsicv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qsvpyljy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vpaymdcq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kpekdrzb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vrwkouwi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mmzmedyk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ofgrenal.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xedcqfqr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2sjqzfiee.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zziinemx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zzhipiit.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wvgbsooy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pneojzla.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nxykssfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgnthmht.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2kjxvoams.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afiklyjx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vuwqoxlj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xpwnhwcg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwbidxvj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ejwvlnve.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hnitoupr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2azphxlwg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2odiavkuh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xnmwaxxg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2euvgveju.html


<!-- 参考信息 -->