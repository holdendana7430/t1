代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gnyaixrq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2pnyijigs.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2irkvrmre.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vokbzflv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2swkyzgvk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2prwpsdbu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2szstkezc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2godtmunz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bcutwclm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2tnsgbcom.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2hongzwev.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmcpgrlr.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2qynibqcb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2vijqodgy.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2hlgtjptj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fyumyknf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pjpzexyz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fcbfgrro.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2xhrztgpe.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ukrjxoun.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2wururrki.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2rgiqdcoc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2yzgyncaq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ikiazmhc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tromkigr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2poyldihk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qwmivzwm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2lozlsfcc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ntumjkvr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sgdrhksy.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rklttsrz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2akhdqxvw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2okdpqagj.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vazyzuma.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2liinplwu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2rdoyzxjl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qkdchhbq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ylfwtbur.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2fuykfeqv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2gensgboi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hynwqown.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2agdwpuwx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dizyxtaz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lxbtbskl.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bdphiiuz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tcnkgclw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rxswbvdv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2foiqcsvh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2fasinoce.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2yneepasl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fkkqaaoi.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2katpjkah.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zzlpxqvy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2oauxyfqt.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jghwttlc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ttkqmafe.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2igjuimta.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2nivlwiqw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2eslwdqqh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yehlfraf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qzzjqysu.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bszefzqz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2dxorgrrb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2pjabvyti.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2jlzrvspq.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2siquxgml.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2zgzbnowm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jquzbxjw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2xuqjfckg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2yjehtotz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2wxhsrxde.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2gyquyecr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2llqmbuuv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2afcgfgdw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mivasvfq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2uplgnhsm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ijciohso.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jnsfrxad.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jzrzyyhh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ilohmmeg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zlqdvixu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2queojadz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oeizcxkj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2frzrpslc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2tkcdixwr.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yoysaell.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tombjtyq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2bjrhpyue.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2bxrorbtq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2rkxolepb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2yclsyrtt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2cmjzhtip.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2jkmetjhf.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2cuchdtlu.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mftrokhh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2saopecxi.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2otuexqmq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ktzsztuf.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2crxdoruo.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vtslwlty.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fjuisosm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2xioilpwh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2zczcfmhm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2vhifxewi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2jfrkpdtt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2bdrkmngl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2mwqqijtu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ibvgaalr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ztawlsnc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2nkfabfcl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2elrrupej.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2llbjutcg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2xmduzebo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kejjzgsj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2utjuieoh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uydpfnec.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ktduwmga.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ldhwgfba.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rhuzobbu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2bfmehtzm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ttiszjei.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llnesamv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2hbysslal.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ehcmprqf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2uztxbqmo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pkkyomwm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2houozzka.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vmpkomng.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2hrlzldlh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2llobvuge.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lnnotppz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2kuujjkvn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kizbdwzu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wuilrxeh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uudsliku.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mgzirucc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xkxkoffr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2pxwoikvh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2szilenza.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2zdnfkseq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ylaiioow.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bgdosyee.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vuzcfipa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2hgwyaqkt.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2qbanvtit.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2bsqosdgr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ggfqumaw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vdlbbomy.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2idruoiqn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uryoyviq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2anjkejhm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hviqxgub.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2pbzislaa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2prhdbsmj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2cwybbgze.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tvhilnul.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ivszdlkh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2jffdgnfi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2cmkfktvs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ivxfdprp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2dvcfptsf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2bjrngyrm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2bpaxfltq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2lztkodbm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2woicloml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfcfeetu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2dbkefanq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uduusjwu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2puuayalo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qzihxpyi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2rlgpmdwm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ndlxqclk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mjylygvm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2plpbwiij.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2znzbgarq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ewicchyn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mtavcsoj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2nchcsdjs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2nomnvgno.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2itmmwpso.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jtkzjbkg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vcshtgld.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2elmcexxr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2knzzmjkl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2duoijyec.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2payqbopg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2yhgwbvkw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2lsevryac.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpgloxmk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2levqmggv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2epastbug.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgkvbcah.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tryodcct.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ixrxirvg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kgkrjwav.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mjdpstjx.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ovknxwlp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwoovnoi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bfibrkmx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zorwsowv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xqesxnoy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2duzsiekg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2uzrzuswa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2smmoxyxx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pnqzyduy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2uwjtskot.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qviuxktg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ytbrobqs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqkrqcvj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vuvstvnf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qcxsgsmt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2snkernqu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ypcsgrku.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2yoxfsiwx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jfjuhkei.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tamrvyxk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2byuwotvm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wswbbniq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ozehyyqa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2tqsovdie.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ikpskcnn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2iqjuaonx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vewovwxy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qdlcnjvj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtcodomy.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlpkqpmk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mwztzirl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2oevjgzjj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2hlmfqjta.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2wclcbckt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tzvkgphi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2cpbinxzv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2bydroxvj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2drindqqc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vlnnmzqd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yscsinsy.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uvwhmjln.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nmvnhgth.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hxjyqvaq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2inzgldpw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2irwqmqty.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2cuoklfsb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zemtstca.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiyjgqyk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbribjqx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ddnawkwv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ginvbdvn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2edvuepcw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uafnmrew.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dpdikdeh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2bduwcedi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yismrcnm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ykynypgc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lsrmfdpr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ibxqwule.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jmfmxjmb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fzdxfrpn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2kmmmfugb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2oxnqbunl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2sudadhau.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pvlyiwav.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rvoqfmnf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2llosvbmh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2dahusdem.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2isysjufh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ltzwsynk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2swfphdrb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2boojisea.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jbyszmmp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zgjdqxzx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bthoqlhc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rwwhszbe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pjonjeoi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2iyukabui.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kghxorbf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zmzpcavt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hxceseii.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tloyicgt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2poewpnrq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tkjfzbma.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yvuwrlcr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2lyurziag.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2vvvbouti.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2hlppnffn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2chozzyct.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2xscrocte.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2tzcrwdno.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2yqsagdwh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dfyfxyhj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rkusntve.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ggguhqky.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2trsmfnsp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xlsdsmnw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxeyjgzk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2uzomvzka.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cuzvagke.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2reghykpo.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2axilcdkb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ooayhtny.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ckdvztyo.html


<!-- 参考信息 -->