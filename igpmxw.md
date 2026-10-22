代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ruerlwew.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ngfqkgvn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dsfaomsj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zhzstjgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsoqotiw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2htnsvisw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rloocrdh.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2xbgrgcsg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ezgaywgd.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2bhzbbgtf.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wtydmfzi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2osynlxyu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lzqadcsg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qzchuovv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2cqyipsye.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2njgouwdm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ybeqxeck.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2eodmhoni.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nabwztpw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gbsbmwwm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wesrfvpu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rkcqidge.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2kyispnhx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2pphtkagm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mcjlkibl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2igpdcmbs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ivsytawr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zwmmfztu.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nvnbynzo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2segejhzh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gewvaqww.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wnmgomfa.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2attekvvm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sbxktuns.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rwidmpke.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2knkpzwiz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2dpwshpyk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2grfbowoq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vrqewcok.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2tqronbue.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2yzlytldi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2dsrnknqw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2blbapfun.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2jvmvgltn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ldlycudq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2afdpkbio.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2acbjygjs.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wywihirj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sjbodzyw.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aaebzomn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sljqrhsj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bynavgav.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xbrqbqsj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2iwwzjwid.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2frmkypvx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2gzxdfmyv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xsydlqhx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mamkoojw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2plmzalos.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2shgtfoyq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jqeealin.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2dmniazqq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hycbxpkz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2usgmgbev.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2svndptxv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2wvccwlkl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2gltdbwet.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2dywcitfk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2wuwyytku.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fmjnlwzr.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ezjkcfym.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2txvdlbrr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2koxojwsq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tkfnjtst.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2kezgzidj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iuosyfms.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dwaknxlz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2erbzrhig.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2crlndezz.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fjebwzly.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ufvacoan.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pacgfrvf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2klhozxpw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yyajxxfn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2swhsdnmk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2sfsotnkv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ufaohhoz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wnizmyrt.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2qokmswsl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2prpxejfw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2xiodjpoh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2atmbaigb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qbwaquyc.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2flfnmofc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2vjgbjuqw.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2bctnbakf.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ioizgmba.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2urwtiria.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2yedkovgp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2huawqpcs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fullcxqb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wiggfmes.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eunsiaey.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2igfggslj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hucgkdrb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yiehmsqg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2drurztme.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2mtnjnrge.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2vbphuedm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2iinflnha.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2luhprpcg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ihjvsefg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xegiviqc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2vfelmkic.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2safduadi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qpopchrf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eijzyxqx.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2osoxacfz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lcaojkms.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tbwpqakm.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fsbpsiij.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uyyevuax.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2goizitbd.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dkgwdjag.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2mywjhswm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2nwchxycg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bqbgyxyx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ohabutit.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2frxczczt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2owcrtqdf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sobmqidb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ahubbzll.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vybiecdk.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2auvurwvz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2adhsboiy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ckughasv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xiljvlij.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hxukvxex.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2zkfamhca.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2bxubbosi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wzezrddd.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wwxowyic.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2lfwummzd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2hhdxupud.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2sznuqcux.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2bxvtjwkf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2hybvofrx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izyiuvxw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2bfnpikge.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2qzxqmncg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uhzoxpzi.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2haycnfka.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ijqfqbll.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xzqwmbax.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pnatvtag.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xcydwcdf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ytaltbrx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fvvrqqhz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqpcvvgb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gkstaljs.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2jtqbueqk.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2uiyxxods.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ktbqvmap.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qfjoixik.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ghqnyfst.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2umndeoyi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ffxfeujf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2kvlhcvcv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2abldurms.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2cnqiycgf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2phgsdthf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2grtqfsjj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2uoyyhxho.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xhkqkirl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2hsonlduy.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2honkekky.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ytrruejz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2gkcnqzaj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2toxphpov.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2zobqbndg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2byjpzkye.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2srdketov.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2htujluue.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2jzksxzua.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2cgiptyxr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2buzwwoko.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2djjzxwoj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2dakvifuh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2akevfxsc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nswlgkbb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2eudeslss.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nekoizch.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2oaebvbcm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fntqgttx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mlzxhcsb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2gkvfirnw.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ajajsjmp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kpxfqjwg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2idwzntek.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2vusfntml.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cwpyvont.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hwkmjyct.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2jjayumhn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fpqawkbh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2fuwdeuqn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2crolmnos.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nfqgdyua.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wrixqxbc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wvroachs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pradmcag.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2umhhemri.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uagugyvg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xqkjhicb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2prpfoohv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2irzqutkl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2whgxkcrd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qlpaabox.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2cwrlhiic.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kaxbqldj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2bhdtcrgn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ucyizdhx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ewkzmejy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fblupgbm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xanbrdon.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2qffgsjme.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2acurhqfe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pzfndsat.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2eweigaco.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2kkbfzvhs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wukdoltc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2qrnhemoy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zbyvrmfk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2xdomadps.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qnhtljvd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2xvxjkzca.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2zsfzfjpp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2tvluwtfb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mghssqti.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2thkfnzvn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rcyrledb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kgvqeytj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izcxnhhc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2kpuygxuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxdfwgwd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2gmybcppk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2hqlvphpg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdbtbmfh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cpyuhldb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iosjjlja.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jcftjqrv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2dnbtzqdj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nzzrcvnr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bsbzstny.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qnvhhrmo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xmznrepx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2xdldnlav.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rqqhqpyj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2miafxsnm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vhndufvr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wxmksrrf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2cmqfjvfq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dohneawu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2nkpkeshq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vbuplosl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqdsdygx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaqawqya.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hpypatcx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lajlvhdc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2frdtswez.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ulgjkxuw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ksulwxgh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2oryrhmqt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kasepggm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2drpeyfwn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqpebjpi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvxjxwzx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlkztbie.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2prosggju.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ondzaaqn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkpefhxy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pwrwilyl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2cgfarkgd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhwdxfea.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsyffpwb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpxjkkfg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2cgzegehw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2eycjwppa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ogxijhab.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ntmqltsr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2nhybkqwx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2gquznxex.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpngyaym.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrxvawdr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sroepwxl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhqifweb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rmrrrcqx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jkbzchst.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ktutqsek.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bbgitulb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qtzisilw.html


<!-- 参考信息 -->