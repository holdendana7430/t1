代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kpkuelfq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wthsiikv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zgamtkxo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pdyqqcqj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qsviipfd.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2atqmezra.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2hvfnibeh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2umgjihaj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kkemkpow.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2cvsyagpg.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gbulwvly.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2uodjmumy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2yzjkjgsj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2tznlzgfz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2fcjuvgiz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2lerbxdwi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ylhfgfcw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rcahfjus.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ftkzrsyt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uatkzroy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ibpzgjfa.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zpwehbpd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tsialzus.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lztsvlwl.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vhsbnick.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xyckxren.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vfdievoc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qajkxxzw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dwhvzuid.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ysnlbmyx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2idrcybds.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2evfvygiu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2opnccatj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2gfdqaidh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2lerrvusz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nphzjizw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2dfvwmagh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2dkxplsmv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2qeqknopn.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2adadpvhl.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kzfgvduu.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2elpmicxf.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2zntakouh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2niecprmj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2wuzifgcv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lilhpvku.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2yxudylyw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kuqlykle.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zdqyjejj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2tpfnmrca.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gsvbgwyc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ctfsrfmw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dkjdezjg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bspluwyw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qbpynfzo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2khiurxta.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uwqxyhar.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2yxosjosp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2kkogffwi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wwylkuhw.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2upurivls.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2oxvkgahz.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2jptqlryq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2igrjnlal.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xcvfgaun.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ypyxqyxd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ohrqrcfy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ekolvkkh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpnpyzv.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2zvzywvro.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uaeiqywf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oxmhfbth.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2detcmspr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rndsusam.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fhlthhjp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2kbjtbocr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xmbkktlq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2perngjnr.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2hfbpuzqj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2kmhttezl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2qttnbvup.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hefrarwc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rfwbevlo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2pyzlzliw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gaqldkmx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2gqsbqdwx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ipdkotug.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fraouwqp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uirrpmla.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zmyydmki.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sopyokkq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jyggzagu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tmdhsxrf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dmqupplt.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hkqjsgtn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2myclgezu.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2moduoijl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2mjallhnl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2twtkpknj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2twnokmbo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2diifqboo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2asjgqotq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mjnmewzr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2pgghjajo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pnxvuruh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2zkhrnqni.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ulxxtoxo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ahohjrys.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2agwszeuv.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2olkwppwx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2qeaerobk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lzyerxgx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tatakprt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2oizbxnbk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qxxlzixs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2wpbejugo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2qzcazqvg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2qhpftiql.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2kdtrwtzd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2roudhiqz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2mbumfxxc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kxirpozp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cahpbzkh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2allozhdi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fxdmdfhf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pllxqmag.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2afatfqqq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gxngtoot.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pzwysvct.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cvbkicxm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xftpksza.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wkdwykul.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2qjgyvomf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vlzgbhqe.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uzjmgbwn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2prcydooj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zfqeyhmf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2tafmklau.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2kzlcodoi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2zbvogpbq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2bnfhyawi.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2sctdlhlk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2utvygvfz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2gyazjbhn.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2djsnzgtr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xtfzqcgz.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2drtxmqie.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tgramqee.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ohskevcn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2pznieksm.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2qtpwryoa.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2mhlrsnty.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ygjsxjua.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2tuyhtywt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2bdxiolrg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2rtcofyof.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2pengkvpn.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2gmgtsptn.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2mebovtcm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2iosqasug.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2xojewlft.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2auftxmew.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hjwktcfc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2okasyepm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jbfwrdxx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hgbzebmo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zopneymo.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2zpdajeck.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yjnkupil.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hfwsazaj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ynsobutc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2weoujoyb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gthjwivf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hqllrrcm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imxmqcmm.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zmsugtyg.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kpgobjgq.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2irtxfrbv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2hkxyramx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2laopkgts.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xfefwiwi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wdwjkydl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vvzarsmi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2agmanode.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2upnpvhsi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2nyltddgr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ccfzutwa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2bqmokxok.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2piiohwgi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2exiauxwv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bpgammir.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kytwrugs.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bchsjaaa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ibifftof.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nlkmlvwv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yqgdljku.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2zhztuhmv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2pqnxmgmu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gzcavfja.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bptzgrbi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2uszwqnws.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sgptlwrf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2rwclcdme.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gubnuhbn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mdlxwyhn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2rvdiabwa.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2oeciqura.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2hmtiwkrp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gighmlxe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zhjusjru.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hcpiifcg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fkavvzye.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2onsygwyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2suiemqky.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2pgrohfpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdxqedsp.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ilprzmoz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2cbvicjop.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2irpltbxw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zrzaqeat.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jwiqenjr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uhkvfjca.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2igptgakh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2rccpcotu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hsjltfjb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2daojcmdj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2puipguwj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ykmkjvqc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ucaopbuy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2haltcept.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uounmqbi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ltucmxfi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2acipkidn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cibwcjeg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2dktuwzig.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2dntvyuws.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hvdwkiyg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fipsazgb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oeuryswz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujhrrlxf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pfgdiefb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2pfjlqryf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zvmjsumu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ezgtkhwm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2sulbaiti.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2vksgxxbj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjwdbttd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxsmwfqm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2rtshucxc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2pvsccbzq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kgfqqecy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gafkvjjv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tuobhjbc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2uprekinc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojrjqyyt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2glaiunoc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpzziqkw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtzzvqxw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qnzsffid.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2tbggwmat.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2yeddsfap.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2suseaafo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2clwzxliw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjoltfjj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nnmxoqxe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ummczttv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivsvdkwe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ncaycuuu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dpcdvndk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2yuddwkky.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2zykanvhh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2enjqskzr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2mqgpmmet.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqcbbcke.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qimhrmky.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vpxxcvze.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gduadfgr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kzoxxnmx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywegyoih.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2wzlmwnou.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ljfdtfdq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yjvmqfcs.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ihocvizj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nzkbugvu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2supzzkcy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2pxthwybm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2tzljddhx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jussoaxa.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2bblcszqu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2xhowzspg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlkzvbjq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jcmwuacs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2occytaqr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jewhklqr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bujpqmox.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2isjxdjvt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyqtnhpx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2nzubswzm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2zqndihij.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmgeugaa.html


<!-- 参考信息 -->