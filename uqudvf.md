代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tvwohxfg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dipziaxl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fuyeimut.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2kptpmydf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ubmvyokq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2affzqdkw.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2azpjqpfy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2edhzrxjl.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ophwvqew.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2hknbdlga.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vfmeopcu.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2imymsbyi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2fqhysnbw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2aobngqao.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2serjqjux.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pwmvtfze.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2jpxfvwvy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vengwcai.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2rgdaryqo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2btfksvqp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yeczpbby.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2vkhipoul.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nmcxiits.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2scmdnfjy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mebdedcq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2stoaihhu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nouepvwa.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2disxxycx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dkmevxwm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ulntsttn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2mlghsidp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gyurdpla.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2mccvmzjg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2lfgqtznv.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2uikncqiu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jdmvqvpz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2juqaboil.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2cfrdkbmd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2iidvtvjj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2lwnxrraj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2nwrlgkun.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2silmtbkx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zixyocgn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fnetuyqt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zjlgwmxo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vsdqvgyt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yfgpmbvr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2xtigyybm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2citedkrg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2raucxrzn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2kvjhtyas.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2qaojxahs.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2zaxnypls.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2pltlurip.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ikvfciul.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cadkoflt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2vwxiaegg.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ivpiejox.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gpfttkhk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2qqkykvke.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tnlulqku.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kczknwfn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nxcohdfj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qbjjkvgj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zsjrmzle.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2enslroqg.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xljxagdy.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lgwjlepe.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2inyktqep.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2mmmqhbsv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jeaorhlx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qkvoecev.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2smqjzuqs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2gzmvrdfh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2viciowsn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2syesfexs.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uhpxnysw.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2etdrfzuo.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ouloiwgh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tsxmcpse.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ogumfpgj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ogtsbxce.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2lsdcursa.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lofjmzsj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gfcvhwme.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hpefyunc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xsbaivwe.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zzjdbnus.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2vvthffxr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2swtmuqku.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2gkeqcise.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsfzdurn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2yotpxcyx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2pzwtwwtg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkdfapcv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2pvljeahu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xzdbjvuh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2isufvxai.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kxxqcmva.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jcfhcxdy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yfcflstr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cjpostts.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gnozjcov.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xmxybocu.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2fpysdxxq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2sqmkcrlr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qcvdblfq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lpnfjnkg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jhtzscmc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2qaptqsgh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2lyypdqis.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2pebfdefe.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2guylwcaa.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2zkslikmp.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2azyzxrok.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2sigiyzju.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fbsinxeh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gfevukpp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2npmwkwom.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ewlmfnjb.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wdkplsev.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2brdulwcc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2mxnicjov.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2byvmhifq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2mszhqmmr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2uezzdtfc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ozczicjn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ljpbyuyo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2cpkwzetk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xdlchjbq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ytjqzhki.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2xkcwuhqx.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2bxqjkmyr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2eypgeoht.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pdhqjwbz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gonawyre.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hkenxknl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bzbktkju.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zlvrtger.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2yzoppodt.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tqadrpoe.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2soydgyxw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2awrtfaiv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2vyhoptcz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yzagvnok.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ctnykotd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pkpzffen.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lwnocbhr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2rmigrekw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dlowjnny.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2iapdunpf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2yswfmhdo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2njvmmfla.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2crueveee.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ilpgwxzt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tcuitymn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rsgdcrhy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2gyqpnamf.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ivfqydgc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2cdibpegz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fwpqwjts.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bxlxmymp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yvgvjavk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2exgmshpd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2tbtwmawt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2lraeutad.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kkckhyll.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tctqaufp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2bfzobdia.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ebjkhwpk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hejxlknw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vpzjbmhv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cozlwgje.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dmvcmrmf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2depkvlcg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2divcvyib.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2lavijfqu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ezpbsqgj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2lzoacfpd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2adazritl.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2hlookpof.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mrpdhhmn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ylkwozgs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fhnwoirn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dxscssvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agmzcgvh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2pmezhyrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yebzzeoj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2stkoceem.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kqzjdtpt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ahyhqiiq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2puffpuyh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uuphgcep.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ureqcbqa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2jfoqzsrb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vykkvswc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lzxsvwuk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2jqmjitxu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uqzcexwb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2palzstti.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vonuvhbf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dcmukjwi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ycrbmlen.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qtzvmwif.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2auhjgdvd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qgjznynq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2nhydpdvv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ybeatxsn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yjrbjmvi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vzponqaw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mupzaqve.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubacpxzl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gkugnelx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2znttsdvc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ujqrosdw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2moyqcsaq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2rxptlclr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2caassjkv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwnjljgb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmviztei.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2wlwawxpi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2uveifhmr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kuvkrpqe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ptfutcqj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yonwycjj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2jwudsdrr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wlzgrnok.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hucxrsof.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ddbftqde.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2paugibcs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2dyydyhdb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2eqhzhagk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2onhtrabk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2cercivtk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2fvwjimgm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2utmzgwtk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaimjzne.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dtvxktgq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hbtdjudd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2yqohfszh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2seayryud.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2zsuvfwfu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2kyoebgey.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2dgmhydli.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2swwdepby.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixlzkfst.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wyrfuprd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xkffnang.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2oayrfvme.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2gzomshxe.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ygklldxy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kqkmgrzl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2twayjpyg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jvklctgt.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zthdfxjj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2onxszqpi.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bbzvefuy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2egnculbi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2lnnptcpz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cgeeqlcp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2lfvvfxwz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tehzyhrq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjdwdkgf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnnycvid.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xufdbcon.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jqtlfwrb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jusruqno.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ccsudxdu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqgjbpfk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2bztzukze.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2uakmvwlt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymhiypto.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lkuupgur.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dtiptyoj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywqnziui.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2cdtitykr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mtpdczlz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2hoajuizb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ngqykrei.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2txsnrlks.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ikvhjsqb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ebcxnpkn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2iavjnlfm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bkqxzzko.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2lepvprvy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gmqzrhee.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uzhncusz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rhhvrqqm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2buyroflh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vevwfiah.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pbvlpkrl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rjzdocut.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xsoijpai.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2tnvywaru.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2vehjmuwb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ahjpfite.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2lackmyol.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2epmsonfz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2fwwynyju.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rhpomnht.html


<!-- 参考信息 -->