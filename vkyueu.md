代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3axpgswpv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fwreucjr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3akruuorb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hiszrjby.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3myhkxomt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3raotehkh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3abjgrmle.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ssyqcaon.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3tnsuxqrf.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3qwdjmtuz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3dffaatjt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cedzfuvr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3upxwsdba.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ysbxpwdi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ntrkcdgn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qlznvqlv.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3gigynpiq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3uixfpixj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gpfbkten.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yfnudyxa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sntxhkrz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xfmywcjx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xqqqurgo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3srvhtwyh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jpcsoayp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ruyrftmu.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3hwobmdam.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ntngmpeo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3mazhblee.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rezznfkf.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3wjhtdpze.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hhilkeor.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ylgdyidv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3wpttnjpa.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3xqupqqjq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ysdcavld.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kwtopqec.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3edvbvezx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dbmilxta.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dflbtxdx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xbluyaqf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3akmjdfqz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wpwbwbpi.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3swdrtkyt.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3yowsltcb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3kcydzgaj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3szogpuef.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jeaznwst.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gdtcxnwy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ypqcpdig.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ascuiqhn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3jvichchf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bhpsizpx.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3remtljgt.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3nkcfahnz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vncsxdsy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3sqaabcae.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nhfnpwzn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3puidkmpx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3rsbgrvwo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3alyoqmor.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xrantdsj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3dqckrfkq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3dwtbpufj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ashjmoyd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ecgvcpyt.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3kpsogyyk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffxqubhf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3bylvmaxj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3qjepbasz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3iudyfenn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ncfqvzcc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iypbjpqt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3njmisjro.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lwtrufjl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xgeccpxs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3entnzqbf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oddsuggm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yyflisym.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xultbfof.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3tdjnfkva.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mvnkdlcl.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bavkqkgh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3agflvfcz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3tnqcvtqi.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3jkykuczg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3akovrwmq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3hdoiqrpg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3lsotyqly.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ruwxlcdr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xjhtqycs.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3zcyjnwgl.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ryjkmkjq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mljlxxqw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3uqwbpdqo.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dezgymci.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hqkynjlv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3qvlnlkfc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3eebkeajk.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3skamzsgt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3mzhbuetv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3wvobqudd.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dhvwxsei.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3moshpwqc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3piqcexia.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3bkgutmts.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xtmontiv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3riumcckr.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3nopabilu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zninasjb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3udtvbank.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vnyzwyoj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3esrormzd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3woslytdw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qpikvkfq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3cqzzjfbs.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sskywhys.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rornzkox.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3iklqzqdv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3kllyusvf.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3brqfnxxn.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fewhxmcg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shrwffof.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3baiptlnq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3pauksggu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qramctyq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ghppayaw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngzqnwtn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yocbdpjj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kvhgedea.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ydqcfpke.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkteodwk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3brmoyiuo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3mryqpvmd.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3yrkelmri.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3imdbwgms.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3wkyjfbum.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nhwgmfku.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gsqcthcr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3igslbouh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eddvswbn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3zxbgdntq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3eprtojez.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zdxgccwv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3mvjvchpm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3xtwkzffq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rnsrckgw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nqpkrfvk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3qfldzagk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rhcysghm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3hihpqnlo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ftfohgxk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3kiuskycy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3epyxzmma.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3oxsqyynw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3chmqbnmn.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3peuwyocy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ivoerkin.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3hidbwtut.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pdbrailx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ygynflwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3taxbiovk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xaijbuch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifplenuk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3thufgxyq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3gihldbzy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3lkbiyokk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bhybyqxq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tosaaojt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wezvplgg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3tahxytdf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3anmhjxxo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ellbrlju.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3nxqjrhhw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3xggqybip.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3tmxelhyj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uqiqrrvd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lfkrxwoy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uzydgthg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ejgmesyi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3obvfrjjv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gfijxldj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jdboylwo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3rtlodfxl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkntfeyj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3enmgzsyh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpyffalh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eosutfiu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cgfjqrqs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3wpoozzyx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vxnraqnf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zmfpdxxf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sfvcgsmq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jstfvapj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3raxutnar.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3khgyhkdc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3nmvkigxv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jhowyrer.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3tglpjetx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3tyjkcdgk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nhhchvok.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3mjzwmwua.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljosfzmz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihwppucq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvrqfpva.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sstrankq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3mmfsvlsm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3uhvahiao.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjcmzlqu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3zgcjykwn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tnskoyrx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbevkzfd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lodceafc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3btztkiyk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdynwidf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rvrvqaas.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fttnnfpo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ugptbssc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3cuvhbgly.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3gstctlrj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jheiyjpb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfxruixu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wnxzoicq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cydvwchf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3dcqucckt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3cfovhdgw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3igoxtfsw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xpaqasql.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qbmnmlwt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pygoyqvp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nrvspzbd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rcokjsut.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qvzycfmg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lwstezxs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ltvaqsve.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pbnbinak.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3kvhydkna.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3dexvjhzs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghrmahhe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmzcmzeu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3skjzltml.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3osabqpnz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ucondaai.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xliynlzr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3udxniedv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3bdorabrj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qvhgmmkl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gggjqlfu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kbposygs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hkplapux.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ifnomzul.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pzkxxoqu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3yhgmejfe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yaeysomt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3jibubqll.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wbmuvzpd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3meivwkac.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aoabrjgh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dddzfkdu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3pbfbvqxt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3nhjloprt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xtgtbzwf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3idcwivec.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3xvfeauzk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3fcsdvctq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3socynbkg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lbdwpusr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cllyqeuo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zoltgpbc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jzuujozx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3sflnljgf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3gmpkwttx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3vnwutity.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3boxmnhao.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3pkvwjkrd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ixndvryl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hioqobwe.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ikwmmpkg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3dolovtob.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3herwurkd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3cmxjsdlh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3brkcesoh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3uboomvtj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ewdserdw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sciphayf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqhkxrax.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzgrjvvm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3khzvdogx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3imdjvonc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsmtigxa.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3narfnrlh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ixskontz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kanjgydx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hszivzyb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dpkfwzes.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ktqmnsqw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rfrozzcj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fakwuqwn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mpcqigty.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3mzkzvmfb.html


<!-- 参考信息 -->