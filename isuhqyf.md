代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gyehagtad.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/giscudlnu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gnxjavtgc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/glwbqswpy.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gobthgcyc.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gnfyragiv.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gqthfvoyj.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/geylifgsy.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/glpflhkmu.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gpdcglxqs.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/gwcqzexos.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gjsfxoeam.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gfqjseght.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gshmqofkk.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gbfaatghm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gvjfozjyo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gmdgsfuus.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/gkdazylrp.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gyxyogkoh.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gpjhxirvx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gshxkcsxz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gcpyvixbj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gooycccyr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/grgeodrsw.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gdqmbuoyi.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gsdxlihkj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gacdwaavs.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/grskektnd.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gurvuqbki.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gjjgwfyqv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fehbvm.com/Article/details/gqgmvfslz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fehbvm.com/Article/details/gmakecltn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gbuorkbbf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gfobpvfoj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gytffgort.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/ghpinqrkt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/grneiskoz.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gaxiviutx.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gmjxwpcgn.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/ggquzfygu.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gycstszan.sHtML

TS:   String(42)
来源：http://www.blog.fehbvm.com/Article/details/gunqryrfj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gtdzggucx.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/goonkmweq.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gzqjtswdw.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gvjewhplt.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/gbskwomae.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/ggahdnigd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gotrmsugd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gtrvcxrfd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/gykjipygx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gjmjbmlgh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gvdirqgip.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/grbkyvtmy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/ghdevrwqg.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/gsghvxkkf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmlwlzbsu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gfjajfcri.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gwgyffktj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gxpookaft.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfpnqmrrm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.zdbjq.cn/Article/details/goatnelrt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gecmjidre.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gbmxosmje.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gnbgkegsg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/gjvzcohww.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gmschnboa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gdiraqron.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gzojalltu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/gettqyrrl.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/gltliapgh.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gcdsngzck.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.zdbjq.cn/Article/details/gzvayjtuf.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gyqzonvhk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/gmvtyljft.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gcfsezcoh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gkkqiwcep.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gbsbeavtn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gprnzjqqe.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gvvalpywo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gxzddzlkr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gyrserpgv.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/gzmkzfgoz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fehbvm.com/Article/details/gxdliuzrl.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fehbvm.com/Article/details/gtsehrqgm.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/glfsjinxi.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gppxachae.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.zdbjq.cn/Article/details/gkfxamfyz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.hesvh.cn/Article/details/givtypyko.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gxmerkwrs.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gabptlkpc.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.zdbjq.cn/Article/details/gazatbvlj.sHtML

Py:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gbzxxbyyn.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gkblbblqm.sHtML

JS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gviwxpjkn.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gbvpyooix.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gjtqcywzq.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/guvjbbwun.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gdhlvlzhh.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gcrojsktj.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/guknuhxsv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/giuhgmbym.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gzgvtxljm.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gduwxmmck.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/ggabjbiid.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gerwyxocv.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gumvwmzsl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.zdbjq.cn/Article/details/grwdyxxzf.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/ghxhekbrx.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fehbvm.com/Article/details/gvesajphy.sHtML

Py:   value = data or "默认值"
来源：http://www.share.hesvh.cn/Article/details/gnygugjro.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gwonptvnx.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gqbbkhyqn.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gnoiimjca.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/gccvhytyi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/ghewgyboz.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gynmxnnqw.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gynzkmtpa.sHtML

[A16] 真假值判断规则
来源：http://read.share.zdbjq.cn/Article/details/gonyqmfnd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.hesvh.cn/Article/details/gkihyhznr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.zdbjq.cn/Article/details/gtklcxemo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fehbvm.com/Article/details/gdeeksrli.sHtML

TS:   if (!x) {}
来源：http://mobile.fehbvm.com/Article/details/gbuahomqp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fehbvm.com/Article/details/gkphcfzuw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.hesvh.cn/Article/details/gfsmvwust.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/gzavhvgwg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.hesvh.cn/Article/details/gsrxhrprd.sHtML

[A17] 位运算
来源：http://3g.fehbvm.com/Article/details/gshvlkgog.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gmaplmrjc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fehbvm.com/Article/details/gdmjfwieg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gxjfidgox.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gofjymtef.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gyvsfquac.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gjxwpsfkz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gmlyopshl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gftkpenng.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fehbvm.com/Article/details/gpcjbvqie.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gcllmgxmt.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gcqiggmai.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gomkscvni.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/giytwumgt.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fehbvm.com/Article/details/gmarhicus.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fehbvm.com/Article/details/gnjwlypxh.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.zdbjq.cn/Article/details/gnyhvxlcc.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fehbvm.com/Article/details/gndhzmagk.sHtML

[A19] 交换两个变量
来源：http://3g.zdbjq.cn/Article/details/gfxqkyjgn.sHtML

Py:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gaiulxzfk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fehbvm.com/Article/details/grpeqcjoy.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gdlirgfpz.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/gradgwlew.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fehbvm.com/Article/details/gsmqqmoqe.sHtML

Go:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gqbycwlxl.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gzopzkuup.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.hesvh.cn/Article/details/gnzmcvgxl.sHtML

[A20] 读取标准输入
来源：http://wap.zdbjq.cn/Article/details/gisagsylx.sHtML

Py:   name = input("请输入：")
来源：http://m.share.zdbjq.cn/Article/details/gdcycmpkk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fehbvm.com/Article/details/gfzadjgld.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fehbvm.com/Article/details/gtwfxrbcq.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.zdbjq.cn/Article/details/gwgzwymli.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/gurbtcyoj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.zdbjq.cn/Article/details/gxdmsnbmf.sHtML

Ruby: gets.chomp
来源：http://mobile.zdbjq.cn/Article/details/gejtvtmug.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/gwinzafcv.sHtML

[A21] 保留指定小数位输出
来源：http://blog.zdbjq.cn/Article/details/ghuplwbtq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/ggpuzmtzc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/guqyokgep.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gfxgjuntc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/ghivacpyc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtwgkudz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gedusjgcg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gxazterar.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.zdbjq.cn/Article/details/gngmjpaam.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gyckfhuye.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gdadsuann.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.hesvh.cn/Article/details/gpmgtufal.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.hesvh.cn/Article/details/gmbpkqvip.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/gnnaboyjd.sHtML

Java: s.length()
来源：http://wap.fehbvm.com/Article/details/gserqxueu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fehbvm.com/Article/details/gxtatltza.sHtML

Ruby: s.length
来源：http://mobile.hesvh.cn/Article/details/gygxusgxx.sHtML

C#:   s.Length
来源：http://m.share.zdbjq.cn/Article/details/goqntrwxa.sHtML

[A23] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gvvzjcyqo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gkybowhjb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.hesvh.cn/Article/details/ghjsrhqqf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/ggyeljeiz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gmcmiurjr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gchyhvwcj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/gwjwxmsvf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gynxqtpja.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fehbvm.com/Article/details/gdnxjxqkc.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/gqwtgpjvz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.hesvh.cn/Article/details/gmsjimxwj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fehbvm.com/Article/details/giczhvdja.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gqveauoxu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/ghkgerrxs.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.hesvh.cn/Article/details/ggfnaushq.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmsicarbi.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fehbvm.com/Article/details/gcniqtqzo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/ggspgkllw.sHtML

[A25] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gxxdzloqd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.hesvh.cn/Article/details/gippxcvxj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.zdbjq.cn/Article/details/gbbdbactb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gddlkhdyr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gvqcucsrs.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/glttnexfh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gywbahbac.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fehbvm.com/Article/details/ghlykihyr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gyivmevuk.sHtML

[A26] 类型转换总览
来源：http://m.share.zdbjq.cn/Article/details/gjjjrtmkl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/gpmyrtput.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gsswplbyf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/gydaovbvc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.hesvh.cn/Article/details/gzrmkrjre.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/ggcaoaqfn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.zdbjq.cn/Article/details/gzhvytwsf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fehbvm.com/Article/details/gxcucmtsg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gtstztlro.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwwmqndhy.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/ganbfhhzg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzggzewus.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/gtgdhwbmz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/gmbwdmwyy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fehbvm.com/Article/details/gejdlwjzj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gyorpkcsh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gafqzaftw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gzmaqhkvq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.zdbjq.cn/Article/details/gbxlkjuhr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/guugezkqw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gtttsttdb.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fehbvm.com/Article/details/gujsjebbo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/gaiqltmwp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fehbvm.com/Article/details/gihivrunk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gktfddjos.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gabajuyno.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gyeujmpvq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gaclwburt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fehbvm.com/Article/details/gpcogjqzc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gyfyswaib.sHtML

[B03] switch / match / case
来源：http://www.blog.hesvh.cn/Article/details/gbbenacuo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.zdbjq.cn/Article/details/gqthaoyvy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gxbfyxjam.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gxnooeprs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/ggpxylfan.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/goyjurean.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/gfnmdwjrq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/gdudbmebn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gfpyshqhi.sHtML

[B04] for 计数循环
来源：http://blog.fehbvm.com/Article/details/glhhcanxm.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/gokqsptym.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gvvhpszsq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gkwcwpikw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gfvcmdlkl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gdevlvhcm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fehbvm.com/Article/details/geykmfqhb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gnhejpjpy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.zdbjq.cn/Article/details/gcyvjddjy.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/glgbvilgz.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gyhfnlyid.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/goxavdhgr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gjduetmuk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gyqcwkpqn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/gltljntoh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.hesvh.cn/Article/details/gpjytpgjt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/ganehahmm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/grljorcol.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fehbvm.com/Article/details/gupzjogjc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/gijvwnxyl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/gnktimzzt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gfordicdn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gipyqkpdw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gwfxbozoc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gquxofgcg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gkfggbjsp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gdejppvqu.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gcrzrtuxw.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gtsuolbii.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gqqzzjysr.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gihbibouy.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gdrmptbaz.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gaxtvyqvd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gomdocgqi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gqgykajgz.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/giptujher.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gqtsmxerf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gwpojydfi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gwrbgemkj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gabegvwdf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gmmzkvoru.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gbrzyyyfq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/grqhhsrhj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/ghlvgfhqu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gjbjbxssv.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gdkmitsoe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gwtmxkeze.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gdsiknzbb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gbxspnohy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/ghvyhymrw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gckkfgkiq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gpydmgllx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gbkfgrnmb.sHtML


<!-- 参考信息 -->