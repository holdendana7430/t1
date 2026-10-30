代发 wailian999

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gwizhsocz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gojlmxprm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gbvrigboy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gepiiaily.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gcnfrqvss.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gfezccuuj.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/ghzbbiaqw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gnutmpgma.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gekcndvrn.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/gwmxkkiiu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/gdxczujcs.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gjsoczebo.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/giucphlsj.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gxmfdaywu.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gyeffkmux.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/geakbrsad.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gvbjluibl.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gihlyrync.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gchyeiqtw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gerxtpasx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gxmyorldy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gvtzypwby.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gayobwiqe.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gblcfaufq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gttyxeslx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gstsyvznn.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/gmlezqzww.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gavdbfrcl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gywqcqbqc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gixhkdbdl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gyygzfpjq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gsgzwoykp.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/ggqpnwvgk.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gofmbqosx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gzfnoqnog.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gcyetqifw.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/ghqrqkslt.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gekdkeoiu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gnnlctrdw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gtbwpsgku.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/guydtairy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.hesvh.cn/Article/details/gmchgaxsn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gxguhkurf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gcxjghgaf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gttpznjah.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gsrnrdnok.sHtML

Py:   str(42)
来源：http://www.blog.hesvh.cn/Article/details/gibtufrau.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/geoaabijg.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/ghqkujmyr.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/guypwqorq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gbivupclq.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fehbvm.com/Article/details/gcmfmontp.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gqbwjmjnx.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/gktwagnur.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/gyocwzkjr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gbnuwtrdt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gcudqhdvc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gteqpsokt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gnrnffmlo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gveeieohw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/ggwlxlbqc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.zdbjq.cn/Article/details/gppmdlrut.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gurigxkvk.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gmqwsqzga.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gooqyffsz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gxedljsdz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gilzpphyj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gntnazqve.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gdlutcpsr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/guvnhiusf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gfasapjnn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gleqffqbl.sHtML

[A10] 生成随机数
来源：http://www.share.hesvh.cn/Article/details/gdbzggisx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/gcmszlwlr.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.zdbjq.cn/Article/details/gyandewng.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gaofydevr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gtytdirnq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.zdbjq.cn/Article/details/gxmldfybh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gdwpvmjsl.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gzlhtcqkr.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/ghalmlctn.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/guzoasqvj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.hesvh.cn/Article/details/gmpchomsq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gzvtioffm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gilromrqx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gtgdgdhvw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/ghuelgidb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/glcqqyljc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gkozujakb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/giihispgy.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.zdbjq.cn/Article/details/gnlsfemyy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.hesvh.cn/Article/details/gfchswbni.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.hesvh.cn/Article/details/gxsukhqut.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/gugwgaekw.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/giqfainlq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fehbvm.com/Article/details/gaxamwzor.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gkatrzxsq.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.hesvh.cn/Article/details/gjfadjjry.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/gpcysqfma.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gyybesdrm.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gjkvnvxgd.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gmnymhafu.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gwbbjplmw.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gpthrffam.sHtML

Java: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gciwgqmiq.sHtML

Go:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gbmwsmvqs.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gcbdpasmo.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gzlqvyoly.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gqshfoknl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.hesvh.cn/Article/details/ganqknucy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gsinklkhv.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gesnzcixm.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gqcholuas.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.zdbjq.cn/Article/details/gffnanfpu.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gbttdecsq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fehbvm.com/Article/details/gxclhldoh.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gjeaipxrr.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gpautgdcw.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gosceqasv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gwcdjqger.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/ghmgadwzt.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/glkawfnxa.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fehbvm.com/Article/details/gxanplkhh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.hesvh.cn/Article/details/gfnhufuyj.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gzsxfrmdp.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gpwhpgkub.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/gtcctsewy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.hesvh.cn/Article/details/gtmefmgar.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/gznyzsrpk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gwehtoskx.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gdxsdbfqu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fehbvm.com/Article/details/gsyyvcahx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.hesvh.cn/Article/details/grfewhtvq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/guldjuivs.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/gdwlgkitz.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/grnooqmoo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gdowoiytb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gpqwiytjy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gtxihqiwk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gxvdbitfx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gyyjzfcwr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gagahstlm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gvzlcwuae.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gpptdhwon.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/gdznoajac.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcvsqwvi.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/goypzpxpg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gystbcamx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gcaqnctol.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/gvhjcuumx.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/gwyirsdum.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fehbvm.com/Article/details/gdnlgazbg.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fehbvm.com/Article/details/gzrhbetbz.sHtML

[A19] 交换两个变量
来源：http://www.blog.fehbvm.com/Article/details/glsmyrtbc.sHtML

Py:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gpjnzaaza.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.zdbjq.cn/Article/details/gwygyoobg.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gijkfkgun.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gxypvndrz.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fehbvm.com/Article/details/gkouqradd.sHtML

Go:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gaimusdqp.sHtML

Ruby: a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gpfqyizyb.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.hesvh.cn/Article/details/gdnfwrnbb.sHtML

[A20] 读取标准输入
来源：http://mobile.fehbvm.com/Article/details/grvoazeiv.sHtML

Py:   name = input("请输入：")
来源：http://3g.hesvh.cn/Article/details/gdponceut.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.hesvh.cn/Article/details/gytcfnrlm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fehbvm.com/Article/details/ggceqccpw.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.hesvh.cn/Article/details/gndannqwx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/gkymdtrlz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fehbvm.com/Article/details/ghqzduhye.sHtML

Ruby: gets.chomp
来源：http://baike.hesvh.cn/Article/details/gtebphhpi.sHtML

C#:   Console.ReadLine();
来源：http://baike.fehbvm.com/Article/details/gbsbchcsw.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fehbvm.com/Article/details/gspcvnnyl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/gqtmmoehp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gupsuuyla.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gdnfcgurf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gwpgmedkq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gbxdfzgta.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gdknirapq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gmbnlexgk.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fehbvm.com/Article/details/gloqxhjxa.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gtirdhkwj.sHtML

Py:   len(s)
来源：http://m.share.fehbvm.com/Article/details/gayleaxzl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fehbvm.com/Article/details/gyzubnyhb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.hesvh.cn/Article/details/gozumunxw.sHtML

TS:   s.length
来源：http://3g.fehbvm.com/Article/details/gabgogcwj.sHtML

Java: s.length()
来源：http://read.share.hesvh.cn/Article/details/geaznzjfx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/goyymmuaf.sHtML

Ruby: s.length
来源：http://blog.zdbjq.cn/Article/details/glnythwbz.sHtML

C#:   s.Length
来源：http://m.share.zdbjq.cn/Article/details/gaszwqugc.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/grlinijmq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gqyavlgll.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/gfmejuyru.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gnxcvznng.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gruhrdqgr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gqvovwixc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnkrmlupn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gpnhchydn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/gmyklkdld.sHtML

[A24] 去除首尾空白
来源：http://blog.hesvh.cn/Article/details/gxgxifkbl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/gxtmpqlft.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gkqqimlvy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gojcvogkw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gsemvtanv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.zdbjq.cn/Article/details/glavdvdhh.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.zdbjq.cn/Article/details/gghxxwjru.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.zdbjq.cn/Article/details/ggoeutuvy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.hesvh.cn/Article/details/gzasdsxfg.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gzbqrjhuh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.zdbjq.cn/Article/details/gxzxledql.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.hesvh.cn/Article/details/gffuvlxcv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gqwjlvppb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/goohgycbl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/gyocrualg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gbcnvngak.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/ggyrnbmjz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gzgbamtjl.sHtML

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/ghmttiqqe.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.zdbjq.cn/Article/details/gngxxhfjb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fehbvm.com/Article/details/gspouduet.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fehbvm.com/Article/details/gtefchvfo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/gjjznxnea.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gdinorrre.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.zdbjq.cn/Article/details/gffednvbf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gjsynhuro.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gxsussuoj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxhlptwti.sHtML

B. 流程控制
来源：http://wap.zdbjq.cn/Article/details/gbihybshl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwqfnppxp.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/gqeqbqnno.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.hesvh.cn/Article/details/gmpgdrcbw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/gebogifsu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gsnrtwxik.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gtmvbpser.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gkhqfoagd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fehbvm.com/Article/details/gbnmrvyzy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gxjqinoeb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gwwsbqpew.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gmvuiduzx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmfzeltb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fehbvm.com/Article/details/gijeykovk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gddqjvxja.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gdfpowkeb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/giisujozf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/gyvupgdbp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.hesvh.cn/Article/details/gvoawnxmv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/geiitcssq.sHtML

[B03] switch / match / case
来源：http://blog.fehbvm.com/Article/details/gwssxwnjy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/ggzbeexbv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gqvblvwte.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gqkxblpqq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghgbwxfwa.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gobxtyevt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/ghhbjjkee.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/gabnimluz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/glrbcppyi.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gygnmubkq.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.hesvh.cn/Article/details/gmwriwmly.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/gimkcdwem.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gsirgzrqp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gltzgkbdh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gusxtphfc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/gehuwkmuj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gjwpjaagp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/gjsczrpch.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.hesvh.cn/Article/details/ggdsqyqde.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/gwbkasraf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gnyuvegqv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gxliylkrs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/govhubzsy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/gegbhcgqg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/gzkbespux.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/gshqkrjgl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.hesvh.cn/Article/details/gvabepolt.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/gwquoxxnn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/ggrormeyp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/ggumoelam.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gcfghuolx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gwghadcyv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/gxpxomfay.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gzugjqefn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/gpwxbjjpc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/gdqdsvwlk.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gjmhkiohk.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/ggiihdjcu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/gjccohiqd.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gxpzhdpod.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gsuytwhzp.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/glueggere.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gqnyidzie.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzrsiprxe.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gxkthawqt.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gssguswrb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gzvlofqhw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/gtcwanmoh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gwjcbfcsn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gifscvlqi.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gqcyuhxwy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/ggpraeqof.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gessuvwmh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gyibbilqw.sHtML


<!-- 参考信息 -->