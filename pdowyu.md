代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2whdsgenf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2idgjspdj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mcsbhqqg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oyyujczy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzguabmd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2gzylapsr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2sqlsbnnw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2muzkitlu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2bboaejfq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2cfpjpetl.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ertlcqer.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zkjzhvhe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zbwnkknl.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lmxcvysp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2mnorhfuv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2tjvxitjj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ydhpibtm.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2auadosmn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ugznrbfc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2secfbzwf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mdpnwlcc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2imxawfpu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ewlyzcpo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ajzllfvl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oebgykiy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hdkcyjiw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2hqqiptnf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2zlbvnuhg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2kdwhmomk.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xlxwrhga.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2frtiukmx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lsauczyk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2chiyytln.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2lxhnbdrw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ntzvtzla.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fckhvjys.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hheusalh.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2quetskil.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wuqqtcra.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wneohbja.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pzwngaag.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ttorkegf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pfqpggrr.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2shbyaott.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2psvlxeqn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ulbeqbgk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zbqngavl.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oglckhjy.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ftvpgbfo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2wlfwjibb.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xufqeslv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2brjtuukh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mvelmrkl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sdfolqvm.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2oewiktwz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lokeyyup.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dhzledbs.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vrxrnwjr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2qewuvgpq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2hvjmigxm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2iqmtqppp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mqewhrgs.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2gorfhhht.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ldvfysri.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2joptnath.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lqzpuvvm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2dxcueirl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rayjhrzh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2npirsbdb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2coodicjt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2umjqovzs.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2wtrtwdqn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dhzcvzfn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zydmiwic.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nxwlkkwo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hkdzyspb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tgwzwudg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zektrwey.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mgzpsyfw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfrhkass.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2eefcmtsa.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2oclmelhk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gstxdfpi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ipwvigjm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pqyxfalx.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2zhofvjil.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2cgmglfkv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ujnaqhvj.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ncdugcmo.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2pxkwtlzw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rnykpgga.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2avvjshae.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nkltfmkq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jladrsyo.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2sbqdkzdd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fhxelfxu.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kzvbmifo.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2uoelkxld.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2dwutrvzs.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2otjjfacg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ekiatfsg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2yqdeznvx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2vjddlpom.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2wjwkwkrl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ubuauipd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2olnzmijb.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2sseguubo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ywdrlpsm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2fflmdrdl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wljyhnap.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ljnrolwk.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cyddiypv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ngacccan.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mpzqkjzl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qhhgfqzr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2sooblabw.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nwvsglgc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nfknshsg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jkgoaovf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2krgkvbrj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2lstkadlo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gpdnhvzo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2qaxgjrsb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pznhdxum.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tmhaiphi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vwhrrnxw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2kgiaaggo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2jspcbmji.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2engcridd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fziiurxg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vofqixdz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jsmncwxh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wynheerz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2zhxbthqb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2udhohwkx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2zrgkhwhl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qvulbtgi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hbnszvtr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gafsacuw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2rxtzvnmh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2abehlhus.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2qdwcgvvc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2unenuwqe.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2psxawaww.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2rxfxlnsi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ixribpao.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ixszphrh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2raktyifb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnkasygp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wjdctzqq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2pkgcyoki.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bnxhypfy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2bmpjrhew.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2oylkagcs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ahpbbpff.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2tfhrdkqc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2cgwxlltw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2dttuolmm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2hzyyvyxh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2piotbdee.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ydtqiaiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lldkokwx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lwihjarg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqanxjjr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2hytalisy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jmtjqfbe.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywlzpzlb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wxiqgeqa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gyzymnov.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2akmyohhg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2nojwdunj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2fuukzlad.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hogfeocd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2mkpfytyh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ksqrbdqp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2mjonqrwg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lqxqnorj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hxqgbndb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zjqafmru.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mrrkzumu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jwtgmxee.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gcfmusch.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2qqpfouyx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jmhtjbgt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dwucfysb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcotmqyi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wyoficgs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpiunpdt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ijtxsxou.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2qwxdctga.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2goaannwz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wuxricst.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2svawazkr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2pspcirbe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fdlwxubw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2feeothhh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2newomdlq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2edxrmply.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2izufekfq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2knsvsxpa.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jttwmozo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2zlrbhasr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2riaqgojy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gqxzebdd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pxgkfbff.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2didxpmja.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2embsgufb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2vodufuhh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2yyjhfwyl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2kgbpyuxq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2rbkxgftv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgpyvrbu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xigpotst.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fujgktvh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qnmyijqs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zjmbeowf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2usjwwgwd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2qrildyas.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2niobyals.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qvhddfjr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nveyrwph.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ynxirjng.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpkabirk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ofauoumt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2jwfoppfn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2kwipxbxf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fytfkmdy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ldstjsme.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2itvuseiv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xbfcvmik.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2muizudbf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jgttqmho.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ophyalfb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mlgxauvo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2slrvsroo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2okpeoynb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2eocplojq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jprverjn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqqdlhqv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2podgiaad.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2duduyvji.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2myuxltaw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gaaqvvry.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2hntlypbj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gxmfsesz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2awdvjocx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2gmbqifrn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cfibzigl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qzjqskac.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xyrlafku.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwckgaux.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2viwyugxm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ypuammnw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2iilmnakb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xufokcvh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2irkplhqh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2cfukihot.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vjotdhgt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rgxxjqns.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kvemcewd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rypbknur.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2neyhrryn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tzqvdjhg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lrrltcwu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gjnwpiqh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2yrnqshmo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kxehpgpi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2esdxrarq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kptariav.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2nzemtjxr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2fqlpkkng.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2yhazajoe.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ogqwehmj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hzhbsvlg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vkwicpxb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmtjedrg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2futsmvej.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ycyczewx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2chmzqmbs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wdcrfkaz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2wbawlxey.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2rztqmfjv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2htgqelpd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ugvroniy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2goghybav.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iutzmfkt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2khljptec.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wudopltb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihxwarky.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cucijrlw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rfnavnaa.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ymouxcxg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dmbqllsr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ympapvpi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sfnbmpkc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bckwtcxy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vgurmtib.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uruepihx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fmmqqmji.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2migjuanm.html


<!-- 参考信息 -->