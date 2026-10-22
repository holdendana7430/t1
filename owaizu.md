代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mprcnirs.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vllbsgan.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hvggvfwl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2frlxixhc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vyihtumi.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pnhjqwns.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vsmndpui.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2zdsjwgdc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxwkffxr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2vdtvvwel.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gcnvgwzi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2abqbcupc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2zpsbhjpv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2wxguvcmk.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2piaojxnk.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2dkqtmhyw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2plkssuev.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bbmolgsf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2itjkjcet.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hgkzgehe.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2flaibfst.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tuvdnnfx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iimtljqn.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2chdcobde.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mdozmbta.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2enweaojx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2lbtcqrls.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rfoizbhd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2irlffgzu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2viffpevo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zboopcrh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2vliqkllf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2taeqoiiy.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2klqtysgx.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pgtrrxnx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rmzmarpo.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dfzdaacf.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2jvwqtpve.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zgoynwyj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2tmfanycg.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2nfbjhjgd.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2obkmcgvg.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ocmtziku.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kvqdddkb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2iexaoqht.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jcrqltoq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2dhwmddpg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2snxekqxc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xhejyeyp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ujwpeckq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ofuqieoe.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jsguvsqj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xxezlunp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2roqnaqzh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2clswywzv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vetguwjo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mmysogwz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2zwfncldp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2qjhldwwm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjrjztgb.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2bmwlclvz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2dwyhobgm.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ynhlwpxg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xixxsgeq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gedxpvdh.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wubpgcaz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2nvuevpoa.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2jeqmeexd.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2fioqlaws.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2mhahphub.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gbxqaaol.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bfjaoepj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rxblqtca.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zjifequl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bkfkcllz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2taxzzjpi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zjrkegyh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jkwkqwbb.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2jozxqhgg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2uxeiamic.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ukzdkvyh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lcdazios.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2deyuezvt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2nvmjtoyb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2vpamffmn.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wzdvmzrj.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2loilznqv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2nydmszdl.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qxdmcogf.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eirckucv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lrfzqaoo.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wgdjzdin.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2occgvqff.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gmcalwjd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xixugoxu.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ybblsixh.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2osjmjdng.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2etugwbwg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vchgkica.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2htdpshbi.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2aseoehjd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2cxydjmtl.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uxbsfxak.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2hudxgmzd.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zrdcpzcz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bwsgbzyp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qmwcgohb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ppkmhbml.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dtrtwwmv.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jloreegk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2whfjgicw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ybxwcwpf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2aplcbcql.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mqpwojiw.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2gqbaurhe.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hejiwxbt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2hrynanny.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2hntbcqsy.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2auyodfvi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uugctlqw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2znfzefxu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2vtlgjeiw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2puljvoat.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2aqkmojah.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2upcuaiev.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vnjwbqqc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jyndhdii.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gdxkajix.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mnrelvgo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oakkcdxb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mvabxjsa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rmsjfeiw.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2jcbybcrx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2rztcsmic.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vdipyxjp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2aeuiotur.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nycnxoxk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2bzqrnsop.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2lwpwlgbu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2pwgriwvo.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2falwayuj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2axcntuxn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2iuxvfwis.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2mhsmydof.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2uecojpsw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nvtpqqej.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2fndmgpro.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2datigyta.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2codtzqeb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2vywuqqmv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2kmucxstn.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2xpffzqaf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2bttwciem.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2tbqvpzzx.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2egxwsuqn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2hdfjlcvg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2jqdktihs.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2lfxsnyum.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2tdgvavfu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2wiebxpsn.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2dfsjnwdp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tthkfggf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuhaarpj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ddivveon.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bghakgtf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cnarhqgd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ukbyqihu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2uyybulos.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ybclmuya.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ybevmmfw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ehbtlflc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2hehsinde.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kssiawpw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2gsykglsd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xapezmwz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2wsvrlupj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2dbguhfhk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qlovpusi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2taqlvgfr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2eziuhmfm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qkyprwgn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vlzqlyii.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hqrdladb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2uzhalfpq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fdtzvhue.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2wgwqlvph.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2uqgqxeyt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2qktziomg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qemnmvzi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2atdrwlbe.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bhwqkgir.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2znflovev.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2fnsyuxso.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2cglgxgxb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2quvstyxm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gcgonvdy.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dkkbmawg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2gjthawmr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ulicbfge.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2frrvvbsb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2cmrqmhjw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dxsjgdck.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ndzigtku.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ccvrrdjj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2hpcnrzpj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2slnjhbza.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2scteirfz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2lwgevitz.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2uxlxxyjz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2iecjfwry.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jmlhekcw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2fiewcspk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2omspjmij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsatvyah.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2slvnskmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kyjextoi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2yrxdywew.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jpuqboks.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2jnuvlsry.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ikckwtpx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dtopktjn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mnhleuxl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2dkaphtoh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2jrbcitux.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qkjrtthw.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2pwvuvxgj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2gujfudyo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ourmcvjo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2liblnfwh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dcxgqgqc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hhnbcmrw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2nxuyjzfp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2eupqniqn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cyvgvyto.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2nrjbcadj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2txleezjy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xwdfjele.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2npekcxwg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2owkgdzkh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fzkqiabi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tzalvpqd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2lvrhkixq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tmgqxszz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mupdsejd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lhcvkfoz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2fddxiokv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvvhtxvt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2acwunvwn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2gkvmkjao.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2koezzueq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ruadmkvi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yyewhwqo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tvsivjsw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hhsnvhml.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpiviqeo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aykqmovt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2huhtsbze.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqlnonrm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kxoavniq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ewadnyln.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ntcaaqnr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ctlxmtof.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2bxxsalnj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ehzqodem.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fqjsskpq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfahzzds.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxginvzv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rpmcbgtn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2urpvtqji.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2szfkdvky.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2gukeacla.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2diweuenb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2lxusjyil.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rvyxfxql.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivljokce.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cxizsalq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2agfvelra.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2qlncludw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gghhxvvs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hkqqvzfg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qpcubcdl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ohejfvne.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nuxmaise.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cprijhdb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ymvjxfwv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rhagvuic.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jgubqdzk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oebpwsfq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qlkyqjse.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vbuankol.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gxzmbczz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2umqqqlos.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqpmvokv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cxtxekrp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2crudzgkw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2uxbqhjfu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xeqwngpb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2budnupuc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tjxaznkd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2thcmtgut.html


<!-- 参考信息 -->