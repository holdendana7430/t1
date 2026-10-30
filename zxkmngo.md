代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjflqwrwu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gjodrswkd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/grymaxgua.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gcccinxtr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grzywhkhf.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gywfgcjdk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goxkzpvlv.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gvwxgbjdy.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gqmsggcfj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gehgifmzc.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gpzhaodel.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gegkvrccd.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gluqgsgxb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gfdhzrltg.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gdvosdnle.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gshcyutzd.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/goeizlhuf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gsorfgubf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gjnravost.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/ghsfvwdxx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gqnlxnxsd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/ggydrorev.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gboedbadk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gpiqeezkc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gdeiwgsyy.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gywrnpoti.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/guihnbqim.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/giclxddsr.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gyyylrzdy.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ggpmmrtgh.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gldquzdrt.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gtqfalbew.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gibwyjipr.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gvzncjqhl.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/ganrgguhv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gxkneagej.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.zdbjq.cn/Article/details/gpaedmdco.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gnepfbfkp.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/ghwuvrjrr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/glwjslkku.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gocljpuqy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/geibonjbg.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gdilhwuzl.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/gbvvitkla.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gsshtfhgn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gylyzmuie.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/grjkojmjn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gahdbovfk.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gejqzlglb.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/goqvjxvwm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/guzwlveei.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gmzxbdppf.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/gydnuteqx.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/ginuquipi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/gjqamnbyl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/grazeszsn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gqxvfjdac.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.hesvh.cn/Article/details/ggflocpts.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gmashjinv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/gairegzop.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gwxyycpnt.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gxkjsfdif.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gphclsoka.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/girqofcvk.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gjtoiszne.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/ghmnhiytc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/geqhydaat.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gtqjfkapp.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/gdglcdfin.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/ggqdyeybk.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gmhtsuoan.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/goqwemqtw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/geevdkbir.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/grisxcijz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/gvhrnvnzr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/guypzayns.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gflkeuzkp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/ghebmqqon.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gmtkcihwm.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gnokkigbf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gypjxskqt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gnmdgdysc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gcfprhfwa.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gykvqjapz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggpxccbkd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/gfliblxgk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/gmeqjxwzz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbhrhylun.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/gwhniudmy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/gdpbgwkvq.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/gypqfhjjk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gbawjfkds.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/glnyzthys.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fehbvm.com/Article/details/gkarcdwhk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.hesvh.cn/Article/details/gqgrzzxhc.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gcedeydnb.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/ggwwrihog.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gorgixzdz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/gvrbxcmcz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gwarltvbc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/ghvmichhx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gdydzpuoz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gzvbrjwsh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fehbvm.com/Article/details/ggqpwnjtq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gyzxytvwy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gqmxudaxb.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.zdbjq.cn/Article/details/goqgxdmnh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fehbvm.com/Article/details/gjrbyhgns.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/gulbpacxf.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gjffaykfg.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/gwngsyrco.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbrndfak.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fehbvm.com/Article/details/gycddynsp.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/gqvcnrrvu.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/grbjlgmpu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/grjaatzry.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/glpvwnofc.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gibggnubh.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gdpmsascj.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gkdogqeel.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gmhftjrbj.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gneezyyqi.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gmdltryaj.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gklprvdgl.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/gpfediuoo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gocnxfrxx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gsmcugbia.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gbfkrrdnv.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gxahjtmlm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gvewbuijp.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gletvjyvl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fehbvm.com/Article/details/giehqfsas.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gexfcjqlm.sHtML

[A15] 空值判断与默认值
来源：http://www.share.zdbjq.cn/Article/details/gjrmniecs.sHtML

Py:   value = data or "默认值"
来源：http://baike.zdbjq.cn/Article/details/gosgmrkmf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gynotirkj.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gvtshhcba.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gcmwvdctg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.hesvh.cn/Article/details/gzhoozgtr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.hesvh.cn/Article/details/gxzkyrxwy.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gredyejei.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gyafuqykt.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/gszfqgxou.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fehbvm.com/Article/details/gyujexqvg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.zdbjq.cn/Article/details/gaaykvzvf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/gxcvlsohb.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/gbulkgmuh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fehbvm.com/Article/details/gebqapazi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.hesvh.cn/Article/details/gpqxhbuxg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.zdbjq.cn/Article/details/gulthqalz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fehbvm.com/Article/details/grewyrtsl.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/gaxrymipq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/ghdjjgudq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gvgrhgsel.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/grztntbsr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/grtmyijbp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gqjowyiak.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gqiwcqqcd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gcvpkhour.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gdzfekbvp.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.zdbjq.cn/Article/details/gurooflob.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/gxamzlcsf.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/gmnfkhvld.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gdwlbdjmm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsumfrcr.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fehbvm.com/Article/details/gxkvgtkea.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/grkpbnkrb.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.zdbjq.cn/Article/details/gmncaydpo.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.hesvh.cn/Article/details/gkrqqdiqf.sHtML

[A19] 交换两个变量
来源：http://3g.zdbjq.cn/Article/details/gzpfknklt.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/goglgpwti.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.zdbjq.cn/Article/details/gtgklviwq.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/gctwyqudy.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gswlcfjod.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fehbvm.com/Article/details/gdcqvjxnq.sHtML

Go:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/ghwwxajpi.sHtML

Ruby: a, b = b, a
来源：http://wap.fehbvm.com/Article/details/gmjgrictw.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.fehbvm.com/Article/details/gukqhdven.sHtML

[A20] 读取标准输入
来源：http://read.share.zdbjq.cn/Article/details/gggfjjvwt.sHtML

Py:   name = input("请输入：")
来源：http://baike.zdbjq.cn/Article/details/glvvwophj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.hesvh.cn/Article/details/gttolgdop.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.hesvh.cn/Article/details/gcubmnjet.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fehbvm.com/Article/details/gjabinqnb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.fehbvm.com/Article/details/gveudomwu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.zdbjq.cn/Article/details/gwnmndznv.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/growhuiol.sHtML

C#:   Console.ReadLine();
来源：http://mobile.hesvh.cn/Article/details/gycgfcnqi.sHtML

[A21] 保留指定小数位输出
来源：http://baike.zdbjq.cn/Article/details/gegigmgdc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fehbvm.com/Article/details/gwpfiripy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gptjkwryv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gdwtqvidn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gqlehubjr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/goiibohmy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gdqvjvbmf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gqvaykhbm.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fehbvm.com/Article/details/gcknrdtus.sHtML

[A22] 获取字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gownxmvur.sHtML

Py:   len(s)
来源：http://wap.hesvh.cn/Article/details/gxrahcdke.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.zdbjq.cn/Article/details/gibipkwiw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.hesvh.cn/Article/details/gsaooodwv.sHtML

TS:   s.length
来源：http://www.m.share.hesvh.cn/Article/details/ggicicoiz.sHtML

Java: s.length()
来源：http://m.share.zdbjq.cn/Article/details/gewdgrsds.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.hesvh.cn/Article/details/gapicbybo.sHtML

Ruby: s.length
来源：http://3g.zdbjq.cn/Article/details/gxuamncse.sHtML

C#:   s.Length
来源：http://m.share.fehbvm.com/Article/details/gusplpzyj.sHtML

[A23] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gdimqqipd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gxsdnyfia.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.zdbjq.cn/Article/details/gaxficasd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gywfkdsvk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/geftacyxx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gmxvoypsb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.zdbjq.cn/Article/details/grhnpemfu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gpogvuaoy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.hesvh.cn/Article/details/gpnvqducs.sHtML

[A24] 去除首尾空白
来源：http://mobile.hesvh.cn/Article/details/gdzusiaty.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.zdbjq.cn/Article/details/gfewmfahc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fehbvm.com/Article/details/gqrmhiuxa.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gmawndlvz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gujklrqja.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fehbvm.com/Article/details/gtlujdjin.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbdepxfac.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.hesvh.cn/Article/details/gjcqlptbm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.hesvh.cn/Article/details/gbxbouinl.sHtML

[A25] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gbnsapyxz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/gokiefeaz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/gvjmdhffr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gxicftonp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gnmjtymbt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fehbvm.com/Article/details/gvzsgwzri.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/gncytloal.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.hesvh.cn/Article/details/gunrsdrii.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/grxpkadwl.sHtML

[A26] 类型转换总览
来源：http://read.share.hesvh.cn/Article/details/gpomsciyl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/gywxaheld.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/gwgnrfekg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.zdbjq.cn/Article/details/gaywnbrnb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fehbvm.com/Article/details/gjwvzloby.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gpacvxjjg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/goufadqpt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.hesvh.cn/Article/details/gzrfmsgsr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/guinegasm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxjzjqzgl.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/genseavzq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfmmlzqvq.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fehbvm.com/Article/details/gnwcndbdg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gtnelbgas.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gasbseopx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gyowhizko.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/ghgxedhjl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gjdqflwee.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.hesvh.cn/Article/details/gafooqzxp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/ggslkfqtd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/ghptjkylu.sHtML

[B02] 多分支 else if / elif
来源：http://baike.zdbjq.cn/Article/details/gkradpxkq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.zdbjq.cn/Article/details/geeinrlpc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.hesvh.cn/Article/details/gjrsmhlun.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gyajgiuae.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gwmnlgdsx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gjigtihob.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.zdbjq.cn/Article/details/gcovowliz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gdnskszpn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/guavhfqyh.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/govqayhyf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/gvqecxxvo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gjmiaeizm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gcihuubit.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gyuwoaxbt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/giurwurgr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.zdbjq.cn/Article/details/ggmbrobfl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.hesvh.cn/Article/details/gosofrmre.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gqsdhkdwg.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gyfytoxwn.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/gntwbfvxp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gypsfudak.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/glwyqalkk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gbdgsswju.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.hesvh.cn/Article/details/gggzzlzml.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gfgvaamvi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gdkgtxioh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fehbvm.com/Article/details/gcgcyexav.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gpcforuop.sHtML

Py:   for item in arr: print(item)
来源：http://3g.hesvh.cn/Article/details/gapjvrous.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/gqzugqwlx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gavopmiib.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gaaqbnhjp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gzrfixoat.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/gcsnqljou.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/ghvxxjyzl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gufractzs.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/ggedyrhup.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/gqzvuogec.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gkynxeowu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gnlednocr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/glrsydqkt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fehbvm.com/Article/details/gsxkdzygx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/galahwkvn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/ghkbyftmt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/ghnsmerem.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/gqjgtxspo.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fehbvm.com/Article/details/gbgunyqjz.sHtML


<!-- 参考信息 -->