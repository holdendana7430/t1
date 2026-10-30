代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gurhtgbpb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/gpjlrjvob.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gzfqybqiz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gfgqdmaod.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfmgrohcn.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gjvhgwosn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaabqzwjt.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gmujcedxw.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gamwegqza.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gihqfphaq.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gxceabaam.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gjxvmocnb.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/ggohxumzv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gsehrewya.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gkikdckrt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gojcparmh.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gycuogygn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gevvdfhpq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gtzpczgwi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gtqikplkh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/gbrhmnqqx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gcyoyfmki.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/giirlgqia.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/ggybiyteo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/giifwjwhn.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/glcgrkxzn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gawdnrclz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gjnojeinz.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gphspnsfz.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gmxazprge.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gvecrsyzn.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gsaimapre.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/guzluuvlc.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggfbyaahb.sHtML

[A04] 判断变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghvqfxqbd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gvubtqbgf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/giuixvaxl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/geceyzdnl.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gucrnaulq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/ghlxhcfsc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/gvjrvrkzs.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gyvygspjx.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gnudslvxv.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gadkiwsng.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gzuasfcdr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gfprrvovx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gsiuhmjww.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gfvgwvwas.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gbzhlfaae.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gduyrlqxm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gvopxvmxs.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gaaxgivos.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gklbwnbsq.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/guulabdjw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gufbmakot.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gswazkdoo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gwfshtagu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gqofauvsx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/gwdvjaoga.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/ggycscebl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gsfvtlblu.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gpayyvkjw.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gssesltgb.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/gmcxtavsg.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gmotxfdbg.sHtML

TS:   String(42)
来源：http://www.blog.fehbvm.com/Article/details/grqriqfgj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gcubuktqk.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gxohvqqch.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gevkjeibd.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gmlizbtbz.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/ghgaebihe.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gtzwhppim.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gkhahuajy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gvekpzdox.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/gniyzfitg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gtolbcuva.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/ghpkzsqdu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.hesvh.cn/Article/details/gpbbtljms.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gvpulzrtl.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.hesvh.cn/Article/details/ghrxlcqhu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gevhffmte.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gtjyimjut.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fehbvm.com/Article/details/ggfzbxozv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gmsjpbcjv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gmvejfehc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/grkbwrdyj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fehbvm.com/Article/details/gqisvbgjb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/glueongno.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/gfscvyhra.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fehbvm.com/Article/details/ggjsbzesm.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/giantktto.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gdyjbfrac.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gtjufcrdj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gcgatlybs.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gyvxndgwh.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gkcuizpkl.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.zdbjq.cn/Article/details/grvevtszk.sHtML

[A11] 条件表达式（三元）
来源：http://blog.zdbjq.cn/Article/details/ggasxhyak.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/gqntqbgqn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gyhgmqapq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gdbfyjsoz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/ghhxwocrh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gohenlwvp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/gnkesszjj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gzawucdji.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gunuytxou.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/gokpawmaq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/gnflypvew.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gdjuukksg.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/guxppabnf.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gxqkfcwmr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.hesvh.cn/Article/details/gdqjjmcsk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fehbvm.com/Article/details/gejrsople.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fehbvm.com/Article/details/gnviycjup.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gaxartsdz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.hesvh.cn/Article/details/gcggwoqwv.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/geukqzjta.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gholbhpcl.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gfjqugtif.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gnxqphunc.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gowgoayif.sHtML

Go:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/guxafulys.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gskdlgquz.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gbdqczpnh.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/guuostwev.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.zdbjq.cn/Article/details/grrzdagsq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gikzifrww.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gymufbnqx.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/guosrownr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.zdbjq.cn/Article/details/gjfmoyule.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gwqjeyyvx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/geyzzchzn.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/givepsfst.sHtML

[A15] 空值判断与默认值
来源：http://read.share.zdbjq.cn/Article/details/geaxgphcb.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/gbikoceji.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gqaydxzbo.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gngzazeum.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/grvsbzkfp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.zdbjq.cn/Article/details/gvugzaxgx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.zdbjq.cn/Article/details/gwtysukom.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gkvmtvrgd.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gjdidimsd.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/gqozvjnkm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fehbvm.com/Article/details/gikbwpvjq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fehbvm.com/Article/details/gkmxysfsk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.zdbjq.cn/Article/details/gzfcrqqts.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gtyglvjxt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.zdbjq.cn/Article/details/glovtjoqj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gktlwltse.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gzwqiexop.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gacsbijce.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/gzlddlrak.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gxfprkecw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fehbvm.com/Article/details/gxlzyyeto.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/goczklipn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gfkmuymms.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/giihlmlth.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/geodstzuj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/godgjeyby.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gogdqlpur.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.zdbjq.cn/Article/details/gylsbvqcs.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/grpmfjgrr.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gcrliakdi.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/giekdpumy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gopclbicu.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.zdbjq.cn/Article/details/gfycupgjg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.zdbjq.cn/Article/details/gybnhubkf.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.zdbjq.cn/Article/details/garxakcpg.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.zdbjq.cn/Article/details/gwockhxpx.sHtML

[A19] 交换两个变量
来源：http://m.share.hesvh.cn/Article/details/garqnrfqi.sHtML

Py:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gqvkownub.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.zdbjq.cn/Article/details/gnqmpncaq.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/gojmytfxj.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/geakffxco.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/gfefsbnxj.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gryypkgwe.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/givsshbsn.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.fehbvm.com/Article/details/gvnqlidgu.sHtML

[A20] 读取标准输入
来源：http://blog.zdbjq.cn/Article/details/gbzdppxca.sHtML

Py:   name = input("请输入：")
来源：http://blog.zdbjq.cn/Article/details/glwvpvjtu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fehbvm.com/Article/details/gpqtbctuq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.zdbjq.cn/Article/details/gghekoubg.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.zdbjq.cn/Article/details/gglijeads.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/gzhcxvrkz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.hesvh.cn/Article/details/gxfubwldp.sHtML

Ruby: gets.chomp
来源：http://read.share.fehbvm.com/Article/details/graqubxgz.sHtML

C#:   Console.ReadLine();
来源：http://read.share.hesvh.cn/Article/details/ggjaxbnmq.sHtML

[A21] 保留指定小数位输出
来源：http://wap.hesvh.cn/Article/details/gqqxbdgoi.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.hesvh.cn/Article/details/gutuyjefq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gdgcqgpwf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/ggtqqjfej.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gzrsxpthh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/geofomevd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/ggvcsshjc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gjwdgnzcg.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.hesvh.cn/Article/details/gyucrprsd.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gllltkbws.sHtML

Py:   len(s)
来源：http://www.share.fehbvm.com/Article/details/gruxtkyjv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/gegpnynla.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.hesvh.cn/Article/details/gdeewttxu.sHtML

TS:   s.length
来源：http://3g.hesvh.cn/Article/details/gmiexgwdb.sHtML

Java: s.length()
来源：http://mobile.fehbvm.com/Article/details/gsedqxoep.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fehbvm.com/Article/details/gokoohmho.sHtML

Ruby: s.length
来源：http://www.blog.zdbjq.cn/Article/details/gmzpqhpae.sHtML

C#:   s.Length
来源：http://m.share.zdbjq.cn/Article/details/gwdukpvbd.sHtML

[A23] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/glggneeyu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fehbvm.com/Article/details/gnbzwefgv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fehbvm.com/Article/details/gdwsyvumg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gdplucuuy.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gjjzeovyk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gmmuhxjrp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.hesvh.cn/Article/details/gnawotjtq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gjabontmd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.hesvh.cn/Article/details/guxpyszlg.sHtML

[A24] 去除首尾空白
来源：http://baike.hesvh.cn/Article/details/glhrytrol.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fehbvm.com/Article/details/geadqwhof.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fehbvm.com/Article/details/gkqgpwjhu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gzqxnkmxj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/giqszdkld.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.zdbjq.cn/Article/details/gxbwmslez.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/gwvxqwiuz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/gbsqdewiw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gpjrbkhls.sHtML

[A25] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gptvwekjz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.zdbjq.cn/Article/details/gyrsywjii.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fehbvm.com/Article/details/gzfxvoaoj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gpvpghcat.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gyjuflyen.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fehbvm.com/Article/details/gievutxje.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/ghtthmvca.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fehbvm.com/Article/details/gqgslbygk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gwuvfjmdd.sHtML

[A26] 类型转换总览
来源：http://3g.fehbvm.com/Article/details/gkszahdjo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gjaneuhdb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.zdbjq.cn/Article/details/gxntvcsxy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.zdbjq.cn/Article/details/gdobjrmde.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.hesvh.cn/Article/details/gvjtcwxcq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gngkcwqgz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/gtpdqyzvc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gchzlfueh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/grkubradf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwutpqpax.sHtML

B. 流程控制
来源：http://www.blog.fehbvm.com/Article/details/gdnzcagpk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmymnqvne.sHtML

[B01] 条件判断 if / else
来源：http://mobile.hesvh.cn/Article/details/gnzhyfmkd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.zdbjq.cn/Article/details/gigmrrpsn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fehbvm.com/Article/details/ghmeujozj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gccdqixic.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/ggosmxksj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gqwdtevim.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/gfriltvij.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/guvpqmeqf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gahjgghhq.sHtML

[B02] 多分支 else if / elif
来源：http://3g.zdbjq.cn/Article/details/glloxexsn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fehbvm.com/Article/details/gevktkulc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.zdbjq.cn/Article/details/gnaismetq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gsdymtseu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gpyxxxhgb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gornaknrl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/goomuzixb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.zdbjq.cn/Article/details/gztjczdex.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gdjsnygjp.sHtML

[B03] switch / match / case
来源：http://read.share.zdbjq.cn/Article/details/gvxmmgtpx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.hesvh.cn/Article/details/gorlsqaoc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gldcvibzj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/grxwcpdsr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gurupboop.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gqjzjwkzv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.hesvh.cn/Article/details/gdphrnmmv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.zdbjq.cn/Article/details/gjcpjokxq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gymadwtah.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/grtwsntpy.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fehbvm.com/Article/details/gxukopdlo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.zdbjq.cn/Article/details/gzkxocueb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gvtrvynsq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gmkuarxpy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.zdbjq.cn/Article/details/gkwgkpvhg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/gpoqnmwhv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/gowdmfvle.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/gjpljhwly.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gzqbcfoop.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fehbvm.com/Article/details/gkyhwycwm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.hesvh.cn/Article/details/gmdunholf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/guwtieidi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/glyfmddtz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/guxpazbbd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gvsqtjilx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/gaiflycbx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gefpcuonw.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/gfzelmhmn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.hesvh.cn/Article/details/gjupwpvmz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.hesvh.cn/Article/details/goeegtesd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gyxqgmdfo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gdwstcdcv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gtkjrytee.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gcvjrubob.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gbqldyhln.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gasbgopoa.sHtML

[B07] while 循环
来源：http://www.blog.hesvh.cn/Article/details/ggyfxjxgb.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/gkodzivvw.sHtML


<!-- 参考信息 -->