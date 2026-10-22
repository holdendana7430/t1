代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akwtymga.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2fxbdwzpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvgkqoqw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2dnljsnfd.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xpphlynz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ozxxxvvf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pggxfryk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2wyopzdur.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kocumqch.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pawmxcha.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2cmourvwy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xzucckvf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2vbqilmqt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ivpdcfom.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2auhkvpgr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dpijkimq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2mzhyqttb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gegzyakr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2akxpvefl.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2uqhcnrjz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xjmqwtyd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ttygesce.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2rsevqddh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vwtohwmz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zzfkoplj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kjefluei.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kkpnnxss.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cxcfzlve.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2couvqtwu.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2blwwuqml.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2fmevmilp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2bxpsqzez.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hhtyciyl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2pkqrmjzd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2otuoabda.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2poizsdbs.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2tbugavjo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2llqwqgqp.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2cnxseeac.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ngnjrdkg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2swepisbw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cvcdnprh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gohtowts.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qbvbcysq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hfurlmar.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yrhnaikw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sokatppw.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sxckuhpn.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gammkyms.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pojrwosm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2shlopnil.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2nsspplsz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2veusxlte.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vpfozbra.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2idemvumu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2gfpulpva.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kzuulmtn.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mwnbpkig.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2yxpsieeg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ouvhxott.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kvqczutf.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bhjodrzy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bvwfdetm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2sbmijodk.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2faipeagt.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2tjjqilwl.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2kcukotxd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vubccdpo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2dvtlzxpf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2snrfrfik.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2hagnyhje.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nvlloogw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ltmlqmio.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2wdeixwly.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2awbhlykk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jqmmhebb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wburntsh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mlcvvpnl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lexaadfj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xabtohbs.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ouyticcj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2zxoebgod.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2grrohbju.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghgyxqar.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2mrhwfank.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2wqmuihju.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2mvlvwerz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dllbxdfv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2devgitzn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2pzkbfazy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2uxiyjbvh.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2yblupdgg.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2acbzaxip.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2djggbwkn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2snmucksy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ogrfawus.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pyplsvcc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lmywgsxo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uexjlvre.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2rltxuisr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jxezjduo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nrxhtyoq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2qsbfqmck.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2oimmlfic.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2xgguegnh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2kmmwntai.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2etwlwrns.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2eqpfmnww.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jkbwuotk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2bupnhahx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2jpfrlrbd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ndrgtpda.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2isstcwah.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bwwbgivv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xevgpbhj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kghhntiw.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ftziccbe.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jhawkgha.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wijgnbae.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jbbufics.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2olfxikur.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2taiggojk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pknpbegj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qvuzysac.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qycruwzf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2qdqkdrlb.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yzygtthv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2kmgldxbb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2csdikyyj.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jlhjqkyi.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vxqmotul.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xhedpjpn.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nmopwrxe.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gjiwarhe.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2qquusyme.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2duknraol.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2guetjdhf.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nyayoxqz.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2rmlimnyn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2xiptiqaa.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2wttdvrte.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2dmiwqnxt.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2quzptpfe.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2uhcidijz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2rgxohrgx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2cqzgicmr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nnxqssww.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2unxiiyxd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wlrurkvc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2smhjhpfy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jdrtjbdn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tjfsvbjp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sdqukeid.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2giniafgn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uwwlycvj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oxsynbzt.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2efjecdtb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uixemqad.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ezxcuhke.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mhicsizg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lhziiapb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2dafhuhuo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2lieozppf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2gwhbwtee.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2lrlophbb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2oukjrlqg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2eaydlihe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2yneilwzc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ktzzpiig.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qavsfcvn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2esdvirhp.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2intngtqn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2svjqckjw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2pnrqyzmk.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2mkunrhrg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2hwecluxk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2xmpnzocv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ycbxfkgi.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ylgusedo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2kvbqmwfc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ytoxcvpq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2dpcqwfgo.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ywwvgctr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2avabvfzv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ivmxxopc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cwmydoar.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xeykhazt.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cordqrex.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ofviotxq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xwjauiue.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ydczkjnc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2exhzbjvv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fbytdmsp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2btweggwo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2rnsezfya.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2pzsiqklj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cdtiduzm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2eqpnzsyl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2evhazrpe.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ekkmvfst.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2qcppgset.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wfvpgcao.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2bknnvxqk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfklsipr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zbwcwqgk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dblvivlm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wvgkrgtg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2wakxxhre.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2enpudkef.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2eusfdoev.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ltxsrxrb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2aousmywp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vnirssem.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bxwepwej.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hvsdtrdr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2wzdzptcg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2alkcdbnd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2mkpmayud.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ifjgchxn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uojaxbft.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2nvmtrnvr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2atfodbiv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vcnulipi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehncvrod.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjacupmt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qeihhish.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2moaoaosp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mxsmynkw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2njkgwwza.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2lllmtmpl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2fegpjuct.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2sqligjpg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2powaqqcb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2psjyptvn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2slqflygm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2pibrbhsh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zonnvtrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtigzosy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ajewvnph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kydepexm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2dlkiesyz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2usywcwpw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfjvdvxw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wrasffsc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hkcbqszm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kjkhhvqr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2rsoavasg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2udqlcath.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2huyxrnqq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2lvpbduoi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xnjmpamf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmsuhphr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ppbbhwzw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hafsjcaw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yodrokbt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2nqjagqji.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jegvyzxg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hmjvestb.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2wjqsslyw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jygynekk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qeakvqdp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zudojaeg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnhkmhko.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gduefhrj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oevktkgm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2oxoihnls.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zdogyhiu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uowmygni.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mubhhjks.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2lljcjpiz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqezkwik.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sphtzxxk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqkepqqo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2lwklnehj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2nijhapom.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ngymdqag.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qzbatiec.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fhndaiul.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wqzmsbtf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2frbeojca.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ulsmhmuo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2blebixls.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2znaxujuu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rgyobrgr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkeyehiv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2kcflnqfb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ndxxbyop.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xwpylbpt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zhfudjsw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqnuqibl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2asoxnvvn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2sjzzlsfq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2olgaxmhp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2cfydtcsb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2drsrhiwf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jgbvgmtv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2widkdlyc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hlvohddk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuxndcxu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eymfbswb.html


<!-- 参考信息 -->