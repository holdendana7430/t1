代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2woymucxl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2jbepyqsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnbbwqgy.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2heemmspd.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2tksdvulo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2pfjldcrz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2idjmfgcm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2fsyjyhem.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rzfcgenj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2dmnaijbu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2tfixocal.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mnsdgbuj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2tsncsfxh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ljtbqeyt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2thvntqeg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2varaspnj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2umphynqp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wfdpzjwd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2plrxfffu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2pvvcsive.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ctecsiqi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2njqsjwvj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2pnfhfzbo.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zjsjsmxz.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wikacaan.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2spbrefen.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oqfvjtxt.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ovuiejls.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vdxydzmi.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qpepbpky.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qyhaqjoj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ouiqbhty.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2kerempri.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2momaakjm.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tfyalrah.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2gguqmaje.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2fgsyjmbx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2vuwjiren.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2xnpgrcmq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2jvnxmwtl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2hkajjnqg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xguhpdui.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mmnxyudc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ofkehufl.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2axgdsoum.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mgyazjsf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2traqphab.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mrmnebgq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mhmsbbwp.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2scjjekls.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2trtuqaqr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2snbfvisk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2awznmour.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2plscqnhc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2rbfuwsqt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2gxakjueo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wpjbgzkv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lxwtclux.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2gngzucya.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2maaqjazd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2dhnanane.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2bzimzonf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2plqatqoz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ncpqxfdb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ylmgpobm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2pgemdymi.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2nzwasike.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kpiiorfc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2wmtkjkmg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zdjyqdvk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2yvlykbsp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2eowxnhrl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xpalewsd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2nvstlgxa.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lvualmrl.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bfpcnzzv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ryybbysh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vplexfaf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2klytegcf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zjobwusy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bnulfyuf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2lddtuvaq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2tfffkgdi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iunyufzp.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hmkaejzz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2bkfezplu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2qsmrsbuk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ytrbspwf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2yrwuadpa.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2aeidcusq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2zuctqcjp.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2zegotuha.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2oompdrle.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2xrzfaetb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vvtdchse.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hkbmvups.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2clipfast.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2frsfmggl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mekphqmi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2qdsikgzh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2udvtzcop.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2emwpfgml.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2nqwrjqzp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2lemiwdbi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2qzpwnmga.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2fhajxxci.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2xlawpxhq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2zynujvjp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2grgmeoso.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2leyskhka.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ptokfthn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zjplfsfv.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wvfsxhgp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uzlrwmlz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cyhezwzk.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xoeaqpse.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qqvlojxl.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hcopcokm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fvexlekn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2djlwiqhk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2cocwqwof.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2yhbucuck.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2aojiqgan.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wwkcduab.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qqjhwjtu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2duqehnoj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bunsjrnv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2mxeqfpgt.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cjwzmxwz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nkvjbisj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2cxgfuxue.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dfdpmqhs.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bmiiesoc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2daqdjyjv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2nbmavosi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2xfljjfll.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wjknwfkc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kidrlzqq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xzchlfeg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2syrhbvaa.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2jxfmtomm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ahbncecp.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jmodxvby.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ombuznoe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2xcqbmbvh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2cqgtrozr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uoedxmqv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2kxxwtfcm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qlaflljv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2otzkouaq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxmbjbdg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tsarmyza.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ujubydrg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jcdpvhal.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cugjjmke.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rpuvjhjy.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2tjjezwrk.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2inevpcyt.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2iqlnmndk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vvhogvjl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2gzfiixnw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2lroylapj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2mdnsllrr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2emxxuhbm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2wdvfnymu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2yhgmbhkh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fnbsfhbx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2yzlzakvc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2fvvkogja.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rmrmebtx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2uqvyokjq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hkdlpczq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tcjycbxu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2pyyvxoyb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2efikgexz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2lveanxxf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2rksygvfv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2kkprnsus.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2foqpiayj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2sthdgxyl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2uhemkhft.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2qzumyfoy.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ieymhqnf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2dnkcqboq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2euhgpqqy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kkjpliix.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjlrfnbs.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2drzdlmjd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yzocclxj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nozniomx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bbhxiivg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2juhvnwdf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xryeqhun.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2xyuspqyt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2hbfpljcg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2bjownypv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zkvoxbon.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2khjmwbzv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nfniuotw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sukjcksz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jezlzpkn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rnozgctv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tgwnqzsb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wawkbplz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aajvlmuk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ovfduqxr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aliyzyas.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rebicqua.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jjickdrp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2munuqrlt.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ymhxkogg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2kmrbixys.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hmczyljv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2swxpmikl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zxwtwdof.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zvrkjtwe.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2itxpeoju.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ysxdzxop.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fgrjekud.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rihaisfj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2azfeglnt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2acmkyrnw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ftcfsxwa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oyknbqos.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2esjqjcft.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2eephjhwt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2rqgmpjiz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2veruekzt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2klaiylec.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2nfymdzzz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2aqkimper.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2nenvccgb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2dxmsmwln.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jujxgxkd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hlofrbzs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2odzljwwt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2eszykivv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omtjhstn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2gxiirfqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iokpmyan.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2yrgieuad.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jmwvceij.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ksoeoypn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cgajkpaq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jmrqptvv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dfrjveks.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2vbkqvctq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2osjyhkdm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2isbgpgus.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2inqnlwbm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2vgcrdgqj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2hztgmksg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ckdivjyd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wvdrwwrl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tkkafkfa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jutknmch.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2tfysfwjq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bfjyhxah.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2whbapjds.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zszdpxsu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqihpxty.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bhtaafkq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pkxwumsk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zwwdliyn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2oaaqxhjm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2kqxuvikj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wzftcwtx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2iayaouwe.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2byuaimcy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2eppainfn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovbbntth.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqimzmct.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2hpwvkkid.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2bxpsmhhc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2jtafsxsk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2aywfzilu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fflucyfl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2yvwwzhwh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2xptvyuwh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qmenvfoy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tymnfszb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvdeqypu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2buymdrmh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2jhkidcwz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xmbsemvr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2hdesagap.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2uilhocgo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rtbotyos.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lipnaefw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rscyejob.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhxnmtba.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ejgednhm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hyjpqgfl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2zgtoazlb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2okihovtb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nmuokxbx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2sswlitvo.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfdthcuv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lswsvsyx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hlnzycvo.html


<!-- 参考信息 -->