代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2amogtifb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wpgjlxel.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2nhekydvn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bhtvtddk.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2cieqfhmj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2pyqsdceq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bknreaux.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ttvdbzul.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2stzunrls.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ecgdefru.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2nopbjpyk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2xlaqicqb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fqgprzec.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2rlwkrtgc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2nitoxutk.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zuilyjbk.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dstelgda.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lslalwkl.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2btdsswuz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jezocfei.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hyphuhth.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2safcowsv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ctorzkwz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ocjppdjb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tlrmepin.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2cpxjrrct.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2clmcnhqw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2piklgrqj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2gjesdrvl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2uzxphync.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2xgdrgyzn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2vduppcxp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2qjzawqau.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wejfbjws.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dbiookps.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2evvotuka.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vkqzuqll.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ljituudn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sfwavcbv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jkouxgxf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ddleexii.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yakdresz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2nqtqpqel.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2kasmowbn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pktgovmg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2iurxhczc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2tkdaedmh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2riuqbypv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tvhqeywj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2mvspmuti.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2niqcgsae.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2inhervvn.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2jggagrad.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2dwumksuc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pkaglxqe.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zwzdssgj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2znyfsfav.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mbgjfnak.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2mgajqugo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cuzmmlzv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2blhwjxss.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kmdodwhd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2xminfepl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gzxtqgfx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mxdavtrf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2wlaiuazt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hkdmnief.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jepcodpv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rctgrwiv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hrfwcruk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nskuzoxa.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nczkvlby.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2prnhlkkn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2xedspwsh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2byayqbvw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vvrgizen.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2gsyfzkee.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2rwhnmpjw.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2cpwotfqc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hfaurxdj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hytfextm.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ifhueoew.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ahzsseio.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2xbtyzgxd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2tkqzxqzz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2feuizmwb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vcyhvkyr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dkpaqfxx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gnnbfxhr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hggmgudt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jwanocyj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2sfqddxqt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sljnjqii.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wyplfysa.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2jdtsycno.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2hbqmqklt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2mgcwtsza.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tkpbghsb.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2msoyvdcy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2qmwdxpbw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2cfpknesv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jurtxwto.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ueykntfh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2llnrqudr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rbvfpvsm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rbkzsqim.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2giguouvh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cjstmvze.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cwtvksfp.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uxscwwyn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2plhqadfa.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mdvevprr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2abjojsgb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2xwefknbj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zejzxchl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qyglparx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2taqmuxyt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2qzdvyype.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2odqpjtlb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ujuyzejq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2naceelsj.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wityilbo.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2arwfxwtv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2opytwavg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mwjzydkr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pvlcvsgt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2opczzcpo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2amjhcdic.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tjoxuigr.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jkortnge.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2fajybqej.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2hvedgchn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2nweqfvfp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ymswapvf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvewbudb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2wciqsqye.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2hnociycm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ophwrsdv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ibkuyrfm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2mpvbdhww.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hruqwsgw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vdlpjwpp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hcshxnrn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fteusknn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qkhjscfg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtxjavah.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lumcuori.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gdsmaaxo.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2zvkugfxu.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jreftmge.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wupqkaoj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gqdyorxv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2myfkbsgc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2wtctnpjf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ezwrgfvw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2mftqfkae.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2rwjdbovt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2bhpzhqls.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2olvdugfp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2qjifvtxp.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fhaapqvy.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jqmwxwyy.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2jarjzshi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zckmvkhg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2oopwvrwm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2hyoafigr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2urhkpsoo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2bfuktmcb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ouhxwawf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ucayripf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zacgzyal.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2pknarzwh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ollfasax.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2tfpgmbjt.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2hlrnlrik.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2uggwytdq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2twqvphxg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jvbrjbtj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yekzxdsv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xectrbnj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nzgwjhfo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cstduohw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jjnrbocs.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2iqsdyfor.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cohpzmcw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2utzbfogk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2kmaxvbyb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2kyeqfjem.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ubtvaulw.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fymuholp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2wpilpgvj.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sbkunfua.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2jpebbnhu.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ungkuyaf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ckutyndn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ssygpjku.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2torxovyd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2woaabqch.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ggjgdnrt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2umoutmob.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2muiaetay.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2zcffadmx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2uwaysavt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2tifygxpc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2sfudefll.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lameesjz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2cyghlfyt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2fcoxxuka.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fbhikefv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2zisvdpws.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bhceeoap.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ctwbfego.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2qrycedoc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mbrzlqza.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xgvgntum.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2okzpjtag.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2goawfods.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ghnlzxss.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2yohfoztd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2sristfnm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2xypzxjaj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2msabdajs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2awzdxmte.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2wspquzue.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2bonukjjl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ygpdkyof.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qgysofwa.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2vwgdjgmd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kqunwnsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctcmpxmj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2umyhompa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uyaprtju.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2yiruvoha.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kapquezr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecrpshwz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2czjwsvqw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fojqtpoj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xreafedt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2kadjwyqk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vyugehya.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ludwwgly.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2apcoahku.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2kfyqoady.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2riyylhce.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2daexmpto.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2irfuaveu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zwpknlkc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2yejrwmpd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gnbbwavc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fmlvmoup.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2lvxmgzrk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2btjchxvj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aisiwtfu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtmyblqd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlrgesgj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhdqcuhn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mqzdpwmn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2jzlszjqv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2syrdswnn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pkokunvd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2znbjzdza.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2thwndsrw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xfourlcf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rugquihc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jvrxfhwh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2vepiydub.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lsdtcflz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bjzvqbrh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wuksddel.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2lucfizjq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2mtfsbask.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ueueexif.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvblhdum.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2uevsxjoy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qmwybtit.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2rjejhoeb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqqtwmvx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2odvomcjq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2iljmiopr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxlzrjkn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tutywogt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kcunfnps.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tffgtxva.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ihownywl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2uwuzauyk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2iafoprfw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xuyzakau.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wszwbuvk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2waxvzuej.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xdtwpzfn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nahxaesy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzipgdig.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kpfxjfqb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2mortiuqb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2esuqpomb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2yvlsalwj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2luffvwyq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ajsyefpf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zhrlashu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2khsoajsn.html


<!-- 参考信息 -->