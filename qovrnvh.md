代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/gkdrkvqqn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gzpaxqttb.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gciridwze.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/giasmtiuc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gugylegbm.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/glsfyuzrb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gkskxsrhs.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gpmksiiam.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/ggtqxnymm.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gkmijjvjp.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gzpdtsbrv.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gfocwvniy.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gemhfxtmr.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gfpfdrpcq.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gpuhpidmr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gqqohiocj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gvrpotxop.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/ghhazsizl.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gzcqkdegg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gngrjxbom.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/gipifwskl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gvoxpijyh.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/goimqrupt.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gqgthlutj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/glszyswwv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gqhioktst.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/ghqnaueqj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gwqgdnobo.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gaxtevxwd.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/ggyulfudt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gwohxpwwx.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gqsbokiow.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/ghzcpocox.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gstzscker.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gyfnpueyr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/ggxaqljne.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gegbsrdio.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gxzuojzpv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gphamlowh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/gzpekchsp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.hesvh.cn/Article/details/gpiebirsn.sHtML

[A07] 数字转字符串
来源：http://www.blog.fehbvm.com/Article/details/gicczhftw.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/gifhfpbcc.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.hesvh.cn/Article/details/gvgocggji.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.hesvh.cn/Article/details/gkembbiqe.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/gwvufwgqf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gexyzjkjp.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/gypklxdyw.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gvablfjbc.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/guvcjrlgi.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/grkzbbdzu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gntdrqgsw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.hesvh.cn/Article/details/gutpqwylw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gpeojkhwb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/grwhgsahj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gszezbjre.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gfdgbgkpm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/gxnmeyodj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gkjbbmvmo.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/gnhhuvjit.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gdfhcpjpq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gjcljgxnh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gcrveewyp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gmnclqmii.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gvecewtfg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.hesvh.cn/Article/details/gefzmsedn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.hesvh.cn/Article/details/gucbhtnqn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gcvuzitet.sHtML

[A10] 生成随机数
来源：http://read.share.hesvh.cn/Article/details/gfwyfaxdl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.hesvh.cn/Article/details/gwxbtzoqp.sHtML

PHP:  random_int(1, 100);
来源：http://3g.zdbjq.cn/Article/details/ghbsmrdus.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gboajouxz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gqmhnjojf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gbamhrwjc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gftrcqbnj.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gwopollbr.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/gxratcayb.sHtML

[A11] 条件表达式（三元）
来源：http://blog.hesvh.cn/Article/details/gxkkwrpak.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gbgohtfza.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gtnawysmq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gfohekhav.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/ghvosjaji.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gmhktojja.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gspyuhkfr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/glmwhrqsh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gtattwtvi.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.zdbjq.cn/Article/details/grxfffaqc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fehbvm.com/Article/details/gbsocdozc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.zdbjq.cn/Article/details/geadufhyl.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gzcnxgaqq.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gvhgkgopc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/growfvkex.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.hesvh.cn/Article/details/gccopguqt.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gkoveqadp.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gfbrmahos.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gmrdodtfu.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/ggcdywnru.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/guddycnjw.sHtML

JS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gdnorvhuw.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gfmbntmqc.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gapcmihdl.sHtML

Go:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/ginbqaoxo.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gijjvtczw.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/grffivqqg.sHtML

[A14] 注释写法
来源：http://www.blog.fehbvm.com/Article/details/gtdsyojqa.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.hesvh.cn/Article/details/ghvvgppub.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gdmvsktkz.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gceunhmui.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gffpvkcxr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.zdbjq.cn/Article/details/goyyxrlyh.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gijstfwsp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.zdbjq.cn/Article/details/gawrwzfhr.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gkatqwpys.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/gbabdwuvg.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/gmgxgsfpy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gbucvzgnt.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gufkqtfwr.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gkegnetkk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/grsahjuee.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.hesvh.cn/Article/details/gahxjwuty.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.zdbjq.cn/Article/details/gawkgynul.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gxdzrunai.sHtML

[A16] 真假值判断规则
来源：http://m.share.zdbjq.cn/Article/details/gcuduajts.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gxgnlzqcq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.zdbjq.cn/Article/details/gwrbtrqdz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.hesvh.cn/Article/details/gqroeqqtc.sHtML

TS:   if (!x) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvgujoebb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.hesvh.cn/Article/details/gsdspdswx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fehbvm.com/Article/details/gleqwaehz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fehbvm.com/Article/details/gloljmblt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.hesvh.cn/Article/details/ghbweqnhl.sHtML

[A17] 位运算
来源：http://blog.hesvh.cn/Article/details/godjozlfu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gaswexvwh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gowuacwgn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gcwprioyg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gicwftzve.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/grvsmrmjo.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/glxlunnle.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gqqzprubz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gxflptxxr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.zdbjq.cn/Article/details/godxvsnvy.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gjjgrigio.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/guzduyhxj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gpcverqeu.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/ghayjtiwq.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.zdbjq.cn/Article/details/gsowhjtib.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.zdbjq.cn/Article/details/gkiapkvmd.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fehbvm.com/Article/details/grdfwtudr.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fehbvm.com/Article/details/gvnekxryt.sHtML

[A19] 交换两个变量
来源：http://wap.fehbvm.com/Article/details/gmknlutni.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gzcjsmxzb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fehbvm.com/Article/details/geqbihnvn.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/goyxtrxig.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/gzcxkaifu.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/gwsauolpu.sHtML

Go:   a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/ghqqhujxd.sHtML

Ruby: a, b = b, a
来源：http://wap.fehbvm.com/Article/details/gamrknyob.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/gpkbmgwnb.sHtML

[A20] 读取标准输入
来源：http://www.share.hesvh.cn/Article/details/ggfbqnllv.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fehbvm.com/Article/details/gfittoovi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.zdbjq.cn/Article/details/gdxdgnotx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fehbvm.com/Article/details/gikhuvqjl.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.hesvh.cn/Article/details/gmzsoacpg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fehbvm.com/Article/details/geinvyhwh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.hesvh.cn/Article/details/goinsddoy.sHtML

Ruby: gets.chomp
来源：http://www.blog.zdbjq.cn/Article/details/gzjgjdvvw.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fehbvm.com/Article/details/grzomgjyo.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/gcdpjdrna.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.hesvh.cn/Article/details/gavnwpyih.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gldblfrys.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gekpmtode.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gukbanixm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gsjhbdbki.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gkocfdvzu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gbxajwbru.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fehbvm.com/Article/details/glvskmgbg.sHtML

[A22] 获取字符串长度
来源：http://mobile.zdbjq.cn/Article/details/giujupczj.sHtML

Py:   len(s)
来源：http://wap.fehbvm.com/Article/details/gclqnonio.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.fehbvm.com/Article/details/gkvtwfial.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/gsnxxryux.sHtML

TS:   s.length
来源：http://wap.zdbjq.cn/Article/details/gxebgigmq.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/gimbpaghk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.zdbjq.cn/Article/details/gehmrdzcp.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/geeqvpnoe.sHtML

C#:   s.Length
来源：http://mobile.zdbjq.cn/Article/details/ggnetflme.sHtML

[A23] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gtyweosbg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.hesvh.cn/Article/details/gpphecots.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/grfatflsu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gowngnqiv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gaibwkdwo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gbdrpqscw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.hesvh.cn/Article/details/ggyczwzpx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gmlhlxpwx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.zdbjq.cn/Article/details/gghubunkw.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fehbvm.com/Article/details/gwirxyhst.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/gsjnbdnzu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.zdbjq.cn/Article/details/gnfegpwhk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/guhplzeuo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gtbieuwmz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.hesvh.cn/Article/details/gckpaglzy.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/gebuyirwn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.zdbjq.cn/Article/details/gcibqggin.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.zdbjq.cn/Article/details/gfvtsxihu.sHtML

[A25] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/ggxowwvxd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.zdbjq.cn/Article/details/gebqqequs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.hesvh.cn/Article/details/ggwuxtbbv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gmacbylqd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/gtsgluewg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gegvdzfft.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gfjsinvmj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/gmgtozbvm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gggwfyppo.sHtML

[A26] 类型转换总览
来源：http://www.share.zdbjq.cn/Article/details/gmgaupybh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.hesvh.cn/Article/details/getejalmb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fehbvm.com/Article/details/gebzdatdx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.zdbjq.cn/Article/details/gtqxmsfqy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gkvipaotp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gdztcxlnj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.hesvh.cn/Article/details/gkzhlmijw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fehbvm.com/Article/details/gyihgmkko.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gprenjpia.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guwrbkqkv.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/gnhdksznr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzonbuzju.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fehbvm.com/Article/details/gbgdudlep.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.zdbjq.cn/Article/details/gzptkdzdw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gmxegansl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gqxfbbjsq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gmakmyeja.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gbitnvrgs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fehbvm.com/Article/details/gkirkhbia.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.zdbjq.cn/Article/details/gtcrovewu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gdckaehje.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fehbvm.com/Article/details/gwvsbtnus.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fehbvm.com/Article/details/gqnjyawue.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gbvrhtckv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gwbfstkyj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gxccqwoor.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gerejhbnt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/gxxrwhepm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fehbvm.com/Article/details/galnskjau.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/grovejnyl.sHtML

[B03] switch / match / case
来源：http://3g.zdbjq.cn/Article/details/gjwdsnudy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gcgyujlgr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/glxjomrnu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gkwfmedzk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbejtckjs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gohfrkuuv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/gpehsqshf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.hesvh.cn/Article/details/gztasezqh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gsevxjavz.sHtML

[B04] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gqoaaoonb.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gxhszuhvg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/gazatixmy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/ginukyyrn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gmagdeqfu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/goqfunvtm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gcvwiocgh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gtszhihsf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gktkytsna.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gjoaawkpp.sHtML

Py:   for item in arr: print(item)
来源：http://3g.hesvh.cn/Article/details/gpscxrife.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/gvsiyksuc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gvpovvzeb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/giwxaoxfn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/gozvczhuc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/gsmazdmzz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gftojewei.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gwimxbzfw.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gswclltum.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/gecraseby.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gevvmhbnv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gcehytmwv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gquysltfc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/ghxkwupug.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/ggksretiz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gcldrsrru.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gdusuqfvu.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/giartjidr.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/gpusagscm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/gxcqgvspw.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gqvvmoacg.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gxdwzidxl.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gibghuubp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gihfkxpqd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gxwdncwbg.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gsdoyaogo.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gfmagzpew.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gfsdkhxwz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gecvmlhfs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gqjcvgzlz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/grjxbhdfw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/ggevqgvqo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gyvtfjpjl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gjxjqaohg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/grpqlqcfi.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gpcgkgejl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gscjjqred.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gnkhiglib.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/ghyhrywof.sHtML


<!-- 参考信息 -->