代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kyocqwek.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xgwmcpsv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2yolstqds.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2obaqjsjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xcskvqzu.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2wbosfawy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nceodiok.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oqhblbgz.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2sgweohsj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2vspblahh.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hcpftkwq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2avgtmypk.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qjryutnm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2brmpexju.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2fqbzzaah.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2itrmfpdv.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ppynqrmy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2fzrleebp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pmfjzrvf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uybsmagy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2kyllpwdk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2twzdreld.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2vehwdqrf.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2upuquvyj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fioqcpgj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2bjlxfgqs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2zualwafb.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hqejojxc.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vtstlkqf.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vljjhxqj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bpgmmjak.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2oxrqotub.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2flrtpcaj.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zvcstcww.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ynrqmpbd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2qzisbrro.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pqfylwsk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wftiqokq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fmfkvchh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2alkqxwej.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2qrzoemgj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2abbcdrmw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2wdsnesoy.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2xgkotetw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2dhqtbmzf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2indhvjid.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zgjludmj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cblglfrj.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wwtrulcv.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2csugbhzj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tzkpirqj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2toepouqt.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xrcvnuws.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2edywzaze.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2utmycpsi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2smtketuu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ziblqkic.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bryxezrb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2bnlcxefr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ivieslmu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2csdasccv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zxbudenz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2fvllruzx.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2iwhcadwe.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wbvwoibc.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2otarxroo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dusiwccm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2xzhmcvbq.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2otzfghqn.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wenbtecx.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2osvjfifm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mvqrzpqt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2exkdlunp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2llzsmakz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2zimyxbzv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uxqdzoga.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hwwzwwrc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2swotbdcy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xmwflmcf.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lomztrqu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gsbftvak.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jswcorez.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dxsdseot.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2btfixddr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fayhzfaq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2yuvkirdv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2eloytovh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxpiodwp.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2sakmrgsq.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2dddmppja.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2jmnpxkat.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gvflgekn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2obcbditn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qurmmxpt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2jzmbadhl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2gphpwnge.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2xuzwdtwn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2tmycnoum.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qordvycf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vfeyvocr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2guniggun.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2limgjtba.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2snqdfotk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ahmiwmcq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rehotxak.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bvfqqghl.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jrxyxhpk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2srtvcwrp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jhguakbo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2kvbdcrbr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2inxurgmd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2robmfnei.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wilaomci.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2mptbtmpo.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2frulkwbr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ayopdrwp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fphtkvbc.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2errifotu.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2znnyjawa.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2agstuavf.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sdyfezbp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jvcdrabw.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2izwxijka.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2advcfgkx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2sxuqbvnj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ztkzzrpd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2asitiyse.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qtuawrsf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wawlseja.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ufmvzliy.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nbwkkrjy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2vzbuqftp.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zxnyuqbq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2inovdcvk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2sumcovyx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ksxhrvtv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jfjygjaz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kzvbgvdr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2hlztmncy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2moskneui.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ykurlgoa.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mtcgklcp.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2fmtihqlh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ppbvvbec.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2zprpfsuu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2mtduwrwt.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2rzfokdla.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkuqcwhn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2nkzjuvda.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2bqzbtqbo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jphxxnpc.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2lpxncpqr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qcfbzsma.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2glygjwgz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2arzotnsx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wzvgtyga.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gjcghmve.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2plninwmt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uunfulkf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dywmuqjz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ikceffuz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2lcliiefh.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dgmastmc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fwtzupzp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2csztvztd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2wxkyocpk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2bwimjenb.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2fbtcysam.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2acbkdvlt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2eytggipk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zqskeqvh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2byarpwer.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tpdjorhd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2oryxyzur.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2hcktkeyy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jvdsnxaj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jklaiuhi.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2vgfddmxj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ffpfywbj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ugjnveph.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2klzquzlr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2apswssuu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2aqjmnpae.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vdfuoatw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ojtgnsyw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2oeatxyoy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2hxxdefxa.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2gyijupwz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ingsyzab.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2trsnzdds.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2idhjhxzk.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2klzszzxm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cuvlmkly.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mbvctewd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lbtktliq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2mrrlcvlq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2evbnopbx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ehxfctuk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2yywynezr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2dwlonxid.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2cxottshk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ozxbggzm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rtcvkifk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gqgyfqcw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dyvngkan.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2puwkwzci.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2otzfxrcd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ftmovhmi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rnayianl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jfeezoov.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fzsktzuv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2badgffef.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hfngeymm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vrgfcvew.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2esnvkidy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2qzqlkhgg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2tooouqfq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ihiitqon.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vbqptlcd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2lrldvqxe.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2mhmemnyy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2zwrmlwgd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kwnebgno.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zxtjtktg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2otclriar.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jzawbdll.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ewvtrfqq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2czynhwfe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2neqsqcww.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2llmdjyiz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2awuhcqfo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbcdkrxq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tbzmxzvf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2otjzqbmc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2tiadwzvp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2pckiaofu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2zmubbdlx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qmrbhiuk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2updnkfip.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mdqigbnk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2abzzahso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxxhkuoj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2vnofjqus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqogtdtg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2uyeknzsw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hkaeyaeb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2eqmmfqyv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fubaamio.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fqboztav.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pslimppj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2dhutdbis.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2enzsgdyb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ahdrwzcu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2dqkbksbk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2afjugpwq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptmnuhok.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cfotdnce.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2urchzxsy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tsmvvwbm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2kkdgrrro.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2skeygchr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tmogwudh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2abycmlqq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2emsydscm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vnnjcahn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aqgthiti.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yvrggctz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pqidvfjm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2itsavsvn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2expnyohi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jrdghthp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bqyigxwr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zavtbzlp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2siqaakuh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zfhospyl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iiwgzysw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2doqjaxzx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2aneijtfs.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ouhqqylm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2zgvuhvly.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tzhbwmia.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wpzvoieh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2fetziwjh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpzzxaow.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pljberxg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hjoiwvxt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ydysnikt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2gtgvkuth.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jorqrzyc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2smmaqvuw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2zgqwyahu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrmiwobu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubakosbq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2okiqqqwd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ygfmvdzz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ixwoners.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2hnxpdlou.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfjdgcwk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rdjsoeln.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wvkibfyy.html


<!-- 参考信息 -->