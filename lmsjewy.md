代发 wailian999

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gqsnnyqaq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gwttvxxnq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gvgkifxkq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gcvsqearv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gmsozpwdw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gwhxxrtbj.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gilawiynf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gxawrkmnp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gwftlfqdv.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gxwrcdxhc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gqpaucnsb.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/glrkasuor.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gagfizooq.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfskglhkk.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ggggcorlj.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gnodschlm.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gkozanhzz.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gmrdjasvq.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/glodnvfaz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gwdvygxtp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gpwrhddln.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gkifppffo.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gwoteapsu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gtmnaqsun.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gzwvrarvk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gwfnsudjs.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gjwjjbfsf.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gltcaxusp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gltimscze.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gyddztkvl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gxxuquzqu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gtzstzcnn.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gfvgqvywr.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gutmhpgyt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gpvgaiurv.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gqpgbicsk.sHtML

[A06] 字符串转数字
来源：http://wap.fehbvm.com/Article/details/gfjihebwf.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gsmjgdopr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/gtqszhijm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gkmcsffca.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gjitbvsgr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gfkfuyrqc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gceifwcds.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fehbvm.com/Article/details/gimiqdbgu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/glntanbgd.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gkvwgzkic.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/gxccwgdei.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/galbzwltl.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/gjrltepqt.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/gwteuydjg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gohmjezva.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/ghjwjkgnj.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/gqxetxopl.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/gijxrvmeh.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gzhlynfat.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gzjwpwcvp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.zdbjq.cn/Article/details/gwvjuaeym.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/glursgfmh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/grqgfcjyp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gxoroxyug.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gjiyhhndl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/gcwjklyym.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gqsynkweu.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gxyakptuq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdimttnon.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gytbcgwwk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gkfddqklu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gvskxzeix.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gzykfvzbs.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/gnrztcued.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/griyevtjs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/ghpdodzul.sHtML

[A10] 生成随机数
来源：http://baike.fehbvm.com/Article/details/gnvibsybm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gookffnbd.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/gozqrydci.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gadfeqyiz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gcivgxocy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.hesvh.cn/Article/details/gsvpcampm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/gkfsohfqd.sHtML

Ruby: rand(1..100)
来源：http://mobile.fehbvm.com/Article/details/ggeyxalvf.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/gfyvlxizp.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/gpnsnmszg.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/gwydbywbj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gjxbbdywq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gsnuyyyes.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/guolqfzci.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/grrammimv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gszpnyqwy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gcovkkihv.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gkbunyzay.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.hesvh.cn/Article/details/gmttxqiqg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fehbvm.com/Article/details/gwpjsrwvp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/grojckaji.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/gdxopkjnz.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gfsbzcspf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/gvaxrkiff.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gvnsrjnmv.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.hesvh.cn/Article/details/gohmpxkaf.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.hesvh.cn/Article/details/gveizzujr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fehbvm.com/Article/details/gytiifgbu.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gvqwxlhho.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gwcqgvwuk.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gtxlnvwyd.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gxzjqjxzt.sHtML

Java: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gtqbduxlb.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gzkyzyxvq.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gfxhmlvhq.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gaujcxypi.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/grbqtewxs.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/gparjkpyb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/ghavttnqi.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gmeewrdgu.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gjkouvhku.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fehbvm.com/Article/details/gepmxqftu.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gojosjjzq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gxurxtkhy.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gljdibiup.sHtML

[A15] 空值判断与默认值
来源：http://wap.hesvh.cn/Article/details/guvrpimct.sHtML

Py:   value = data or "默认值"
来源：http://blog.hesvh.cn/Article/details/gllnqnzig.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gcdhjpvrv.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gculvtcdd.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/glxcddeme.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/gfexwunnp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.zdbjq.cn/Article/details/gtqrzlwov.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gudjhqwra.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gjhxtxsau.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/gnyxpfzql.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fehbvm.com/Article/details/gypjeourz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fehbvm.com/Article/details/gwnhkpxdh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.hesvh.cn/Article/details/ghydkbapk.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcuixlvqs.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fehbvm.com/Article/details/gnfoxnyxg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/gawjddrst.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fehbvm.com/Article/details/gdhplbhgm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.zdbjq.cn/Article/details/garlgaciv.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/gtptfkvjo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gddbgqnwj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gzswvoqff.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gsaorfump.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gesaznqiq.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gbjtnfjzd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gixibkllg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/guscrpcwh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gkpwfmlrd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.zdbjq.cn/Article/details/gkzfstgyi.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/glcxwflyu.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/gjdkbyeab.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.hesvh.cn/Article/details/gorffcsce.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gufteopkq.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.hesvh.cn/Article/details/gbtqtceuo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fehbvm.com/Article/details/goostvalo.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fehbvm.com/Article/details/gnofnocux.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.fehbvm.com/Article/details/gqsznhvlx.sHtML

[A19] 交换两个变量
来源：http://mobile.fehbvm.com/Article/details/gpzklnttf.sHtML

Py:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gxibhtknq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.hesvh.cn/Article/details/gictvozlj.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/ghvijjbje.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gikpyoxbt.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.hesvh.cn/Article/details/gxwiyxwya.sHtML

Go:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gueucqtck.sHtML

Ruby: a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/giynuuwpm.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fehbvm.com/Article/details/gsycaxkbt.sHtML

[A20] 读取标准输入
来源：http://read.share.hesvh.cn/Article/details/gtweycvqm.sHtML

Py:   name = input("请输入：")
来源：http://www.share.hesvh.cn/Article/details/gvhphsquv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fehbvm.com/Article/details/gzlmuccja.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.zdbjq.cn/Article/details/grruahrzw.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fehbvm.com/Article/details/gdflqhptl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fehbvm.com/Article/details/gdqkypeuw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.zdbjq.cn/Article/details/gwqlevdoq.sHtML

Ruby: gets.chomp
来源：http://wap.fehbvm.com/Article/details/gzrgwkpmk.sHtML

C#:   Console.ReadLine();
来源：http://m.share.zdbjq.cn/Article/details/glkuxuqmz.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fehbvm.com/Article/details/gkmobqwlk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.zdbjq.cn/Article/details/gsuejxtfk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gissbljto.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gvlsjzhfu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gbtmpjovf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gbnkmchdr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gfrtfrqvc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gymwxbvus.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/gzmfeuycq.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/ghzjoelxx.sHtML

Py:   len(s)
来源：http://wap.hesvh.cn/Article/details/gjsvblrda.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.zdbjq.cn/Article/details/godsbkqnb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.hesvh.cn/Article/details/grrlgcpxt.sHtML

TS:   s.length
来源：http://blog.fehbvm.com/Article/details/gpespdfdh.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/gncueshna.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.fehbvm.com/Article/details/gseiadvwb.sHtML

Ruby: s.length
来源：http://m.share.zdbjq.cn/Article/details/gwzxlvxrh.sHtML

C#:   s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gjdengyuu.sHtML

[A23] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gxhvpwpcc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.hesvh.cn/Article/details/gzcqgdtbr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.zdbjq.cn/Article/details/ghyheeosi.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gvhublfoy.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/glnbdnrka.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gfmsuwcrp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fehbvm.com/Article/details/gvzpcicgy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fehbvm.com/Article/details/gqvyfospn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.hesvh.cn/Article/details/ggcmqfiik.sHtML

[A24] 去除首尾空白
来源：http://www.blog.hesvh.cn/Article/details/gfeltcinh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.zdbjq.cn/Article/details/gkaalzsmz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.hesvh.cn/Article/details/ggyvkzvwb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gnbkzctmd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gvjkjumit.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/gxbomczww.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.zdbjq.cn/Article/details/gmfulpomz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.zdbjq.cn/Article/details/gkevlvkhl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gdvtkohmf.sHtML

[A25] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gpygmmzka.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.hesvh.cn/Article/details/gpgbajbcs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fehbvm.com/Article/details/gqhlydisy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.hesvh.cn/Article/details/gdszkhgeq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gvthajvbg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.zdbjq.cn/Article/details/ggtrlburq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/guemmpzlo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.hesvh.cn/Article/details/gnbgaeaml.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/geraeyehy.sHtML

[A26] 类型转换总览
来源：http://read.share.hesvh.cn/Article/details/gzamfntpv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gdvymnhpr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/gzblbxejh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.zdbjq.cn/Article/details/gmfhkfksj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.hesvh.cn/Article/details/ggycikvvm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gxbmjxvoz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.hesvh.cn/Article/details/gbmzcwngd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fehbvm.com/Article/details/gnylysoqx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gdhetkyze.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gracptdus.sHtML

B. 流程控制
来源：http://read.share.zdbjq.cn/Article/details/ghbausito.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfajpklfl.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/guroovrzv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.zdbjq.cn/Article/details/gboxihneb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/gukupghsu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gerxzqsos.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gqhnywpvb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gympjhzas.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.zdbjq.cn/Article/details/gvzzljrfu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.hesvh.cn/Article/details/gazhfuujn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/guqedhjsm.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/ganworlaa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.zdbjq.cn/Article/details/gajvpwqgj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/gxtuxueds.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gosgpgkzl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/ghdrtouov.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/guwmxexol.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/glmfnxzje.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/ghyauyhqk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gupnpxsby.sHtML

[B03] switch / match / case
来源：http://www.m.share.zdbjq.cn/Article/details/gbkvdgfam.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.zdbjq.cn/Article/details/gkhgmhwmt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/guzvutlsz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gcfoptawa.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/ggiqbplks.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkxgxbgpq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gshqoihij.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fehbvm.com/Article/details/gsohjqfjn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gwtkemirm.sHtML

[B04] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gmdmisgui.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/grgcptxjd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.zdbjq.cn/Article/details/guyjhjwby.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gplntwmph.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gorcfrile.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/gbgkuasqh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fehbvm.com/Article/details/gssnvyygq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/gbmgatqvt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fehbvm.com/Article/details/gbjwubyeu.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gwqokqsef.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gmgpvxkhl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.hesvh.cn/Article/details/gvijemlhv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gxgqhvbrg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gkuvgoixo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gsqakzttj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/gnxiqiosh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/gmgfrvzgq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/guhbgafzi.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/gwxkyahtt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gyxkcaqon.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/garamnfhb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gxapiqfgz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gbijytlvl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtibtwjrz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.hesvh.cn/Article/details/gsjirmmwo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gvfdwioom.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gkqkjzycc.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gzuhcdjnv.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gljhplxlq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gengshlgk.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gtgqepgte.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/ggmqfmkyt.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/glnshhobv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/gtzwwpeka.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/geknoznva.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gjmuhsugc.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/giiacleqq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.zdbjq.cn/Article/details/gadfwxccu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.zdbjq.cn/Article/details/glmenboyw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gwnjogjhy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gmaovdkzj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gnniutrlg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gmytwnpta.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gaikqaicl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/goaugyxku.sHtML


<!-- 参考信息 -->