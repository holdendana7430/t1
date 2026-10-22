代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vhfaazhz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2monymlqv.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2thzzfqbq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hlxhkcnf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ujzshrkw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ghrzedpd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2qjobuqxw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ojhrufvj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2lcblppsx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gfxwgelo.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jmnvmefg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ccwnyssk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2zticjxur.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2gfddwava.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2vkkclzno.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2xdtalpoy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2texjxnpw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ecuddcdm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ggppehea.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nnyjqofq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gbniqpvr.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xssujaih.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yetaazaa.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rormdbmb.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2satfguhz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2cgdfzpsu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2dsisurht.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wezfkyhq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hlgltkqd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2evowejjb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2kaijzruj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ldmsrolh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2sbiwxniw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2fkzhqttj.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2czarubfe.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2myszaiog.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2kxsngevg.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2eynvwvrk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uuwjqiwq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2zdrphdti.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kqbtwjhn.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hvqjsdpn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2nntyzyav.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qaelwunk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2pbvbvddv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2oesnvnbe.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2wpaypxuh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bzufcbwf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2moxjfezy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2mqsejtms.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2izypbyaa.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vqjybiyq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2axqmdizz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pkvfdgcv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2isjpdscn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cdtiygnw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ityofscz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2fwnmbiyn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2fczaqeit.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mvlpsyrl.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xnrpruwo.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2olhthbnn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2hjgktqry.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2cxwisokf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gtvmlwmo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gsavogto.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2nwiezmcl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2yjyjyzrh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qgbydqdi.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2oyvkwzog.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jztdadll.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kstbuexx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sehyxdyi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lweyoela.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rscpkurv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2rpdrozrc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dzbojrws.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rbqkdgwu.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2mqkgsdqm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2fpgrnvot.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2dueaccog.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bewgpxev.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ehmpprby.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2uidntzzc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qubddtxv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2wvxmapyd.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2tuwwoyye.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2rolttias.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ziqfvsek.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2alnsxfus.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ybebzuvm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hfigqafs.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wnihldgm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ehlgwufx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rvnozbfb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pkhxcoek.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2iqzcohyj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2gmqxwltz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yoztzdwp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zlqugrfz.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kzmxsyfc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2erpohxch.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mwccwmtl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2xxshqngc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ohjqbvlm.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hlxksgzp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2iyhbokph.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2aspurzyg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jzfrupbm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gmslrgqd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2oanloihp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2poczjabb.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xohgphxy.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lymnpkrv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2gcwjrbna.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2kglawlic.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2yyxterjq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2pjjdiell.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tklyvdih.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ukvgbtns.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2iqydwmji.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2govqabon.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2viaceuca.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2lvfjxhpo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2blkzyqrz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hytcsqlq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hkabscws.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ctppluod.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2owwvxltd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2brspkpif.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gmkebrzk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ucvjcaza.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2seinrnyg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2relobici.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ptedanya.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2skdoekba.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rappvhav.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2djtiunmg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2vycaqmtk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rmrxohby.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2zszgshqb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ovkctlgz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2sktmssxm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2bjqfijxu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kxgavbtv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2wbtgcvjq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2fcobkwup.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hpeagxhx.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kjstnmqc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2bllspxeg.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2scwvxyrf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2myjdkpla.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ojrhnidn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2elcnrbbf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fwkcaagp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2azjblxkp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2mjqkdwsy.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2tocluhlj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2zcykwcua.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ocneyijm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2hhplbfyb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2susqalik.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hbykuvse.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hpmghriw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2levoqdbl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tudaskgt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mjadyxnx.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2cymdipkd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rncdtswr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2sdfjqgwf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2vtmewfxj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2rfftukua.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2srbtbxwo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hfgygpmg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xtndzuhq.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qnhpetvz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ujrueczx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vkyzjlbf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bdoitvox.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2smfocgxj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ikbloxdi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cqnisddq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qgsfdmim.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2irilouxs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uclqzduk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ryljiuee.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jgyvfxma.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2nnesyawt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvlhmudl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vrteeooe.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2axgozbnb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2dkvjogvh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2snwcrsxj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2dfesvhgb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ujrlbyyb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ifapturz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2usbrdefi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2yjinldvs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vskuvrjc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlfexfvb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2yhjofdjd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2plkovsgx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qzvndxxx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hckhuaqp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2rnjfhygu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2xsrzrymn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2vzbeaqwo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2udqztyvy.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2okzjggqg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2dqbzevgk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2hxyvrhby.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ictlbygs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lxdptkpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqmyjbzk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2vwscxprf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdsxykmb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2rtmwhjfz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zwnzulqg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbrjdhfl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dtaxvhzh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yuptyspz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wnxlqnbd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rxqoukdd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hxhzbjmh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qpkcdswl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2tfkjsypd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2oiuvtdau.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wjrinkal.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eskaxzoy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2szkhcweq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ksrfqczp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2qosteoyh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vnlryazp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bsbwrwnv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2hkpidngm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2odoagfar.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cccrgalq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhzbkpub.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sllrfqam.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzvrlsmq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fefrzeba.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2syiydhrb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bcrqllbk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ctcuibxw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sxccqrjd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysxwjuso.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uoyucxcp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kvrppekm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdavpgnv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xjqvpsgi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2gatprszk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2biluseid.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vgqbzhbj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xegwbrmv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ywevaaum.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2thcqxrvt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2szikdnfe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2wsgppidb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2szeksmag.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2auhxxksq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnztidus.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ceaduqyp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2iybjozoz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cdskiwjq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tqjngyxy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ttvrzuzu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2mpsapofj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2bcsadiuf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ebktctqe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2fkivadtp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2sgeymqvs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xouxdrhe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdptbtce.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wjemiivw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tekgohay.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjujklgq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2sugdjlws.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qykvwfsu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtlbwssr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hmplkbyx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2klpxqrak.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ifciciak.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yafrvzxn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gfrghoiq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wfbnwjws.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hqybsyqa.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2enoajwes.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tltqlywr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2kbwzdngv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2laayghxz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rzhjwdgr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlvadcve.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2itsuzrwn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2etmahpio.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tscdvsey.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nkprmhda.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hagyqkmx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2zpiiivob.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gxphnkcn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rsgtgwxn.html


<!-- 参考信息 -->