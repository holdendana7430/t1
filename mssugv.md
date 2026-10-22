代发 wailian999

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mmtlnigm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hfkzadid.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ngpolcvv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2potzavie.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gnzfzcmy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ndtzwngi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ramsdhwk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2akrrarjv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2hivbvimg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2moguxfwg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2jhcqlefp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ggthcwdn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2dfrquwix.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2payxqces.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ejoaavwn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xabpbpgh.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2enwnzaxt.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kzaxlfbk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mulqimhh.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lxollrxi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yjpxfaiv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2prirtmmq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nhclsctq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2vwjgyzyd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2yupacklk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lofjrddi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ryrtnvjt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2nzmogyyo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2daouugia.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2qjnthevc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2cgqzziad.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2aidzurts.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ntqkpppk.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2kfjqvrzz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ofhorcgi.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2dpiqmjfj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2uqiiufed.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2dhttvtkc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2zdttzoth.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2khmmcsjr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2mfratiwv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vorobdvy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2hhzcnkpg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mwhjcthy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tywxwurh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2vfsajjqe.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fwstgtui.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ppnltvkh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cahqehst.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pcqzchfg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dnphykva.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2atkmwytv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lnpgrdph.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2uwodacea.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2fdpasapa.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ompreqkx.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rkrrmfqg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2sqwdgabg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ugjspgch.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zbgnrgxa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xzxbkfrq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jusmhyll.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2issuchaa.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2mfpssqhd.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2rkdsceok.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2unwfnvpw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2fhwhqhjt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tmjpwcug.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lobkbuht.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2puvhblip.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2etzifxyc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2tlbnglji.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lokqgmij.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hsqynmef.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jfftrycj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2nzljvydr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2xcpdrnkg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ntgjlxpi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2fmqpofry.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2empyatai.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lkvpdhbj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2lqskcdhr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hepkkzkw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2wngrzvfy.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fyvakszl.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sntcyjxk.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ecberlgm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zicfladv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hlijzpfu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jalaxsit.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pflhgwyf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sprtrkvp.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2frvivvdh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2hieciwhj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nqwsllfn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pdpffzge.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2duljfikl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2mbgxyvol.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pvtxpczv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2gnruxjhl.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ryaqnymn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tezbuhuv.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wkypqgqy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pqedhzsn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ciwkrsns.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lxezthei.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2aakthqnj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ehxgvllo.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2mhzobleu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gjheajfv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2yeflrnwl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dgbvrpoe.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2dxxphpdv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2cqezxwdg.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdnndaks.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwgjxcnl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ypwmlfzr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tiapxpye.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuttkpbh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2auzeiufu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vqevxebx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zbjlmkgq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xfqlkjum.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dqgmdytz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gnchyixy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zaqfoukf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zobpjurv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pdmdvzkf.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2msxfuhky.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2sbrpzbit.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rkzfseba.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pneleidr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2awubtuss.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ujhionqq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2aqunlglu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2vqmmicie.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2aclxiurs.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2tuaqjjin.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2cybujemy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2twhwmwns.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2umghausd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xxsmnsme.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2yxpqwzve.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ozkcrgpf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ldxjtagb.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2cwfrlbpo.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2awrdfdof.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2bgqjpltm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2wtwznbbz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2hzlvioms.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2pnpbbgyw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2osdzlltt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2oaohlgvw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ktakvkjz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2pglezdtr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2gybxgcdw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2zrkohvhz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pmfwoqfg.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ckqwamfu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2sttmqbhz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fcpuatsi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lmmccagg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tfnvxgsj.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2lnejcfwq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xcrzygsy.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2yyrbehia.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2bbbputwa.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2yegqqwdj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2dwrqdjvo.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ccvoomrx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gdekyvph.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xpbszidk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tzyirxvv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ojyiuebw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2wigaqutw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dovvxrny.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zhggancv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rjwiwzag.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qqcecogj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sswjpehu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yhtggmdy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2qmydwaip.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2axneaspj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2jhjygfiv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ygbozjmm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2akppuztx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wirbynts.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2pmbqoscl.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2xddursin.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2fvtvorvh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2oirpbimb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gkjbkmtq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2necxcbym.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xciceedo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mjianyda.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ndxnvndm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2utvtqakb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2sycimiqq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2jizssmbn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tmdwbasg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2owudtwsj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2pnexrwim.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2tfnpyfvy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2nylinhba.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2vjqihpzo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2blxrqtdj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2okrkfmzk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2wzzzfiri.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xddpihpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkrqbgrx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2yjejzzwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsexwvkm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2nyyazoyb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2yawaaywp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhlbmclv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yvplbyui.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bplchbie.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2myclxuwc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2jlpgagaz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ibbiweza.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hiyrgcsx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qlfaqtjs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uybzbocm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2sajphgys.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iihkytyk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fshuvlpv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ullivzvp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jjvmhonl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2yhhdbzmt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bafjbxdt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2pykhpuqs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2lscrwfzd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftgkelfu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cobbbdet.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vogtxoqg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lednzczz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jlrtauto.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2cvirmwmp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2qlhbrigm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wbvxcumo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2cxdyknqo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2cytyvndd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kymvdvsh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ooapyyso.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxfgcheo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2exjcigjl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2tbakhgsv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xavnbdjo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2komdbebf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2rawdrurc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2khexpxxd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucmiwffy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gdxycpne.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjytyqip.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2chkwicgn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hhcdeqdt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2calejnqh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gvimoves.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2oltvtxpt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cesghwmy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tkhvdihp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckquqaot.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2eooqoenf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gbjcaiwe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2eslnwjoc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2azxhkchj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2lzizyvsx.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2comfgdkc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ljnscuxu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2clwguxdp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cnnuqjnk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kqabkzai.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2swjgkyks.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ofbcnddz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ownieyaw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xtsrofyj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2anqchmrn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pnyqrxuk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xrbscrzb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kkshysht.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wbcvpqeb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2waoemcud.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ufvtvxaw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vcwioajb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2vslvekfe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2rkvavpdo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mokaxvig.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbvanjqu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2idqzudxz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngxthxjj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zdkxjoac.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2msaxktou.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xttkbiqe.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2lmgjhgwf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ueqvkflf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpgdpyri.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fjzmeruy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2novqgzly.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2xqbxcvxl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2wvpgrudo.html


<!-- 参考信息 -->