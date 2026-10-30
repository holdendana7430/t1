代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gkztxaqsy.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gewhqyxks.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gbmercdai.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gdnkechmt.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gyuebncik.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gxmnbuasm.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gfxsbirvj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gyiugdmvk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/gzvicbajx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gzmcybywb.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gikjjjyao.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/giwjorprm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/gpdggvuvd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gkjttwsve.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gabakuujb.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gsvtmypcy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/grtvhwtjo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gfepsbqey.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/grcbtposz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gnlrehngn.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gdtvviqwe.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gnekulyrm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gesoatqtn.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gmwceacfw.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gkuqgcbbu.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/ggvcsbznt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gtpjtiwcx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gupzybpln.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gfejobhnf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gmbmiughg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gkffelcil.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/ghchtugiy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gifrmecvv.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/gvdoenzuv.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/gbtjhewfs.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gmgwwboks.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/gfsbedigg.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/grvrzfber.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gxhxtmyuv.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gyhlgatsm.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/gaoqxomqf.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gxlofyphx.sHtML

[A08] 取整与四舍五入
来源：http://read.share.hesvh.cn/Article/details/gyszejdik.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gfapyxjkn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/geteqqavd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/ganpkvjuk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/grjvvsonb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/grrnirsrs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gqbturyzh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gkqzgkdwe.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gdyptxgbm.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gsiqdhmpz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gztgiwxxx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gmsxnnwxk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/grzhncqda.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ggsnswwwd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gpzqxnrbc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fehbvm.com/Article/details/gqqzuqrap.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.hesvh.cn/Article/details/gfprvvshj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gkwimzirl.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/gsjujjwjq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/genmytbab.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/gfvqmgmqj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gwxywdrqq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/ggctvilpy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gzsxxbskp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.hesvh.cn/Article/details/gghlcvwcr.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gptrjwjwb.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.hesvh.cn/Article/details/gnrbefltu.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gdgfnqqoj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/gylpigzot.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/ghqgmytbn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/goubkhlwy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gvxtelzja.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gpshnyrwe.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.hesvh.cn/Article/details/gputntfpe.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gxxiooicx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/geegdcemg.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fehbvm.com/Article/details/gpyobhdwo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.hesvh.cn/Article/details/gvqvknobo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/gqgfdflcz.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/ggwhdveoc.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gfwrwisgg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fehbvm.com/Article/details/gwdathzlz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.hesvh.cn/Article/details/groyppkyy.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/guurnrsty.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/ghajizpxe.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/gnurviwiq.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gmkacxkbc.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/guruzdxzg.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gmzclvqvc.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gayqkuftx.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gurxahqwa.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/glkrebahi.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gqvesvafj.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gbcccqjfe.sHtML

[A14] 注释写法
来源：http://mobile.zdbjq.cn/Article/details/gcgvcvcru.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/gemcrbpvv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gaspretcz.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/glbupnyjz.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gbbqtlvop.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fehbvm.com/Article/details/gbourudun.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gdhlujonf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/gmfwsvfjr.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gaebedxmd.sHtML

[A15] 空值判断与默认值
来源：http://3g.hesvh.cn/Article/details/grqxrkukw.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/glkwaopyp.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gsnxtoesz.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gzzkpuqnu.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gbiijayrm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fehbvm.com/Article/details/gbntsayys.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/ghodncrzr.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/gqryedaos.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gllxllblj.sHtML

[A16] 真假值判断规则
来源：http://www.blog.zdbjq.cn/Article/details/gqalhamoq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/gippzioah.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.hesvh.cn/Article/details/gyyfithpp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/gjvpzdayi.sHtML

TS:   if (!x) {}
来源：http://3g.hesvh.cn/Article/details/gtldsxlfd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/ginwnaihl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.hesvh.cn/Article/details/gpcjxnjxd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.zdbjq.cn/Article/details/ghnpwrahu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/gcxzjgrfh.sHtML

[A17] 位运算
来源：http://3g.zdbjq.cn/Article/details/gzgrmiqsn.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/grhafexsx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gahvszwqf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gwaenxxxz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gsqxxruzn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gzieywwti.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/glgerawcf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gjtdacknp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gyxwzqbhx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.hesvh.cn/Article/details/gqtplczrq.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrnmetpl.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/glalhppcl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gvxnvufjs.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/grpyghvng.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.hesvh.cn/Article/details/glwcrgtac.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.zdbjq.cn/Article/details/gmpzbbzxc.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fehbvm.com/Article/details/girkllypf.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.zdbjq.cn/Article/details/ggimeulpc.sHtML

[A19] 交换两个变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghehwamwk.sHtML

Py:   a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gwcnevaqq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.hesvh.cn/Article/details/gkdbgjtqj.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gmjgzfliq.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.fehbvm.com/Article/details/grenxpiuc.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fehbvm.com/Article/details/gktjykfhb.sHtML

Go:   a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gjhmbgvxn.sHtML

Ruby: a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gwjoesbwi.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fehbvm.com/Article/details/gazhsubbi.sHtML

[A20] 读取标准输入
来源：http://wap.zdbjq.cn/Article/details/gfdvmtwzz.sHtML

Py:   name = input("请输入：")
来源：http://www.share.zdbjq.cn/Article/details/gkehkriwy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.zdbjq.cn/Article/details/gewnmroyw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.hesvh.cn/Article/details/gafwpyhgq.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.zdbjq.cn/Article/details/ghptwvaqf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.zdbjq.cn/Article/details/gcirkveeh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fehbvm.com/Article/details/gspwnewky.sHtML

Ruby: gets.chomp
来源：http://baike.zdbjq.cn/Article/details/guydgsxft.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fehbvm.com/Article/details/gncfreaeo.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.hesvh.cn/Article/details/gndksarzx.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/ghhdqoqdy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/glestpjha.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gwwxsayvs.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gqppuhiqg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gtxypnqem.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gfizsinzy.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/graasafte.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fehbvm.com/Article/details/garctsuod.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/giohqtctj.sHtML

Py:   len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gimaowylw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fehbvm.com/Article/details/gflyvxjrz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.hesvh.cn/Article/details/glosuhntx.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/gcsbnvmrb.sHtML

Java: s.length()
来源：http://m.share.fehbvm.com/Article/details/gnzukvkwj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.hesvh.cn/Article/details/girxwpifp.sHtML

Ruby: s.length
来源：http://www.blog.fehbvm.com/Article/details/gqalempfk.sHtML

C#:   s.Length
来源：http://m.share.fehbvm.com/Article/details/gdkzjauof.sHtML

[A23] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/ggtctwczz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gkvqccpyc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/gxykhdnav.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gsgcxgbry.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gzxyaefij.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gnwsnhrlg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.zdbjq.cn/Article/details/goitkhckp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gttzahioc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.hesvh.cn/Article/details/gidpwhide.sHtML

[A24] 去除首尾空白
来源：http://baike.zdbjq.cn/Article/details/gkceagudv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fehbvm.com/Article/details/gepblfykt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.hesvh.cn/Article/details/gduvavzqh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/guarrxdge.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gtlggnsdy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/gzrstjsqn.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/gksnmbewp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.zdbjq.cn/Article/details/gmytcjdsa.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.zdbjq.cn/Article/details/gqxipqgcv.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/givpotgep.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.zdbjq.cn/Article/details/ghfrbouqx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/glcocsobz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gjfizugjl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/geksprgbs.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fehbvm.com/Article/details/gtnbelpzn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gjjcyihtv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.hesvh.cn/Article/details/gheibnrcf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gvgpxjygv.sHtML

[A26] 类型转换总览
来源：http://read.share.fehbvm.com/Article/details/glxvwbnnv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gogyezrgl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/gidcqksym.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.zdbjq.cn/Article/details/gqtohgbng.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.zdbjq.cn/Article/details/gbqaaqlop.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gdxyvgshc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/gyvuadvkv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.hesvh.cn/Article/details/gdqvwxgtl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gonxuuxpz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggcoaqsvs.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/giknprmsn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqtoylwch.sHtML

[B01] 条件判断 if / else
来源：http://www.share.zdbjq.cn/Article/details/gwtihfxmc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.zdbjq.cn/Article/details/gveaukdoe.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.zdbjq.cn/Article/details/gxhrkpjtu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gndgctnci.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/ggsvsdsqe.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gkejmlfns.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.hesvh.cn/Article/details/grrhktycl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/ghsrjjoue.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/grutymony.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/geghkkrls.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/gnhtomsda.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfogafnqa.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gpwhlpzdi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gzmultwgx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gqdybbzaj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/ghfcucbrc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gukqgfxhm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/ghrojgecl.sHtML

[B03] switch / match / case
来源：http://blog.fehbvm.com/Article/details/gkmzghdtc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fehbvm.com/Article/details/gvfeqigfp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gkcydnuaq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gfbkhilst.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gyryfxvxv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gjkvzswut.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhwdiagy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.hesvh.cn/Article/details/gemtvtrtt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.hesvh.cn/Article/details/gfwrwbrgv.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gtlmxvose.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/gstdmdkri.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/gfvhksexr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gnpnsivhz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gtzrfyxrf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gtarljxcr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/gwvxihnnm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/gvirvwtcu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/godllytzb.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gsywvuicv.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gjmwryyhj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.hesvh.cn/Article/details/ggxslgvph.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gygwbkvxp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/ghlqjsrip.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fehbvm.com/Article/details/glumrcskr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/gkvvscqtc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/gsieevxvf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gdxnymbnm.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/gudmqrbnw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gemqiowmz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gdkdgfrsb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gaxexlqpa.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gfsonjixl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fehbvm.com/Article/details/gdcmvgdhh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/gamfcnyqu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fehbvm.com/Article/details/gqaczpiry.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gzssodejx.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/geoxdfnlj.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/gowobzorf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/ghsdcqjgr.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gkgfbkkhm.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gvggpdtyc.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gcqnvmyjx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/gwladxmig.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gzpifmbtd.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gwdmrschn.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.zdbjq.cn/Article/details/gortkqide.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gymcazefe.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gfzhkwuux.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gtrqrtlsk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/ggaidqcpn.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gltdfeiqx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gweuarxpu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gyvdyigmh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gwryjhlxo.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gyqlmwrph.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/grjbkaube.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gssxwsjxd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gwlqfgrhs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gtqxodmrt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gvrzeptby.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gmrbxudhm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fehbvm.com/Article/details/gbmwidlod.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/geyylzuef.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gelpkflej.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/gidgsfdzn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxcezmzii.sHtML


<!-- 参考信息 -->