代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kzwopvsq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2qkeakbpa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2iinoqnoz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wbgqzunr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nedmksfa.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pdbdzxto.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zptmurqz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vcuddlhp.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2bnecihbj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lbtbzwrj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ketbwrca.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2lrnsnbof.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2nlnqybwv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2bdcmujuk.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2cgerwxrm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2orrzxbka.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2mimjecrp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2cnpuscjj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2prjdcpiv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2uifzqgeu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2catnmjag.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2iuftjych.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xycaurma.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2egikibsl.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2alptwnik.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2adljwvgv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jzrqnjdb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2itogvaaj.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2oznmedpe.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yyiykput.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2hwrmbpxs.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2fdzmmefp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2jyveibot.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vdutdpvz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qzhqbdfq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2mbosgnqs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2mvatsbrj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ivwbidmj.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2inbrlcak.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2knjrfahf.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wxcvpdma.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fjymrbrh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jdiwzkwb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2sxlhkeua.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2cnbpfjee.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2uemjynos.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2dykdddcv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xjjcdrwn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2wqwjszpy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2thvbzcyb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2rvhqvvjf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mkxcmuqb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ssitexhd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2vlrqcmlx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mkdvodhi.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xlgudyek.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rxapdxpp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2trdupdih.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bkeztexk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sfadkqhj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cyorzyck.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2mjcpkpvb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2wrfoisws.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nrnduvna.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2tfkytxgh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2rybrpcgd.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2tmhokxri.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xzpknayp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lrtszipv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2thiiqosm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2cothbczw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ccodmmfp.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2emhuhxoc.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2jugidkcs.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ifxhmals.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2smjcurro.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vdglqxct.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fokeejer.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hekbevam.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2irlmoqos.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ukefishs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qfduovrk.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xvblauhj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2vqfltqhp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2usjxrfne.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zmixmjxt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bvntwysb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ehalaozd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yqouexrx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dqxxwbyo.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gyspetfl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2uzzccqff.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hbkwltnl.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oasqocns.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aohysddc.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kqlbnmxt.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nzosmcwa.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qlziwfhn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qoqtaxiy.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zclcmcsm.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2nbxwswpj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2nrqcseia.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mhxgdwkt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2chqjpzqw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bojyxyxm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2pyctxxsr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fiifbjzv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2tskjrnac.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pxsnxxer.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mmnpojog.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lwjhvezo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2prsfpqpc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ftwdmtkh.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mzqmxfxr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2arvzotln.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2cugunxkv.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tuvliwlk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bsgbzxqe.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2koexkqdk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rtnaibvt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2wqsyyhrp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2wfapdtpr.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lsntklct.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2dsaytfxy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2xawqukfk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ahczidii.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2aqwwjjwr.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2onsdbdzw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dgaqbmza.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bwmqogsx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kjfudpms.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vyhfpxty.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2txiphfbw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zjldovdy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mznazcyv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iokhocsl.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2mroshoka.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2kwkikhrf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fzgfhzhx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kmnkkmgq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hzdwwgtz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2rhgbouwv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2rxaxfisw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2aiqumlkb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2tlcnxpip.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2xmxuzhrn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2izplxzhh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2cxtirovv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ifqrbncj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2vghosmjb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2vnuxkaip.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zjgrqlvk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fupyhabi.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2hckedfoi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2sapqkhwt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2sanuwcqz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2wxmtvrdt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2lbyduczp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ygruvtsa.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2cuplmfpo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2mbjwzadx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2keojwqts.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2wwdrjokc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2gwflhzni.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2qjoyshxx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2orzvzbli.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yoxwgjaj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hmwkwdgr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dqqdxbeq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2eaikmzox.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2btpupvxa.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2cmnsvkod.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2osbpoxbw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2tjytczza.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2qsxbyepu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ltbgudey.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qmjfcpbm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2buxwnnwq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxumnmke.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nmrjdtoe.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2fzctezeo.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nshulxdp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2onsvecsu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2idiqbqps.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yhgtacph.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gqnpgvke.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bkeskdlw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksnbvomy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2sqcouzfi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2wxbdvmuf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2uxgnvvgi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2qxutgeor.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lzygkjxf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2munjlicc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2naykskbu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2isqfeldi.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qwpjawlu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2tumxvxku.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kwxoceuk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pdstmaye.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2guhycuqf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2inznxzpa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ghnalxbe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cuiboltv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2tehnyufh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fdnvgthy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2nasolzdd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxdebdyq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2wovmycpt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2xcdkhetr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2abrmxmgr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2insuqcoo.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2irmodcxq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yagnvqfv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2yceasugm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2vyonccnl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fcnmmmir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhpnzosg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2idkzhulr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqzztfmd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ixynsjju.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2utsilqfw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2vrdoguyx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2opoxltml.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mlunsadq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ebdhosiq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2pukfddsd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wvoamoqo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2olhqandr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2igpgkmad.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2fhdytqyi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chwnllxz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rpfyspne.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2skxdtwzh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yodvcvoe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ivvhpamn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2rhiyeurd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jofczazz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2hrqjhtbz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2nrwlbtya.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymmdfvjl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecocvauo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cdeufrfh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajmlpbxy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qvfzelai.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2duoiijxc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xmxguqxw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vjcrgkpg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fitmdvgc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2nuymjgkn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nyoovhjm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpqaeljt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mctzgvlj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2wistypwu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kocxnzks.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2lsbuxrmj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ohdxozjb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fuzjfleq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2odogqmxu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zjfaxsfm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbasfhfg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zscvogcv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2shygstes.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2lxzftcmo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2hxketkjv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2hicqbjsy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2lislodyt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfxurfrk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tujfmowj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jxtzuzjz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlwscmlv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2icmtolmb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rrkmoirn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqlvxqvn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2urfkbsra.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2egghbidg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ueyvyhug.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2krfgbvbt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwvhhxtl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2slqxhnip.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2vzeemwhn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xijymlsk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yisgkodl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2notvzvml.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2fuarsoex.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gyoqljrl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oqllxozn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bvnfqwck.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cubefipr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uxrwsdtp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2dvlfnjja.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wysgospe.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2exjrafnp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gxlwllli.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yrvszlpe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vlienflk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ujkgaskc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2opndytox.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kwxmfrlr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2cgrzpshc.html


<!-- 参考信息 -->