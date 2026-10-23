代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hfdjyqbn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kjmleoyy.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3hrbkbsoo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3rrxnxikq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3phplhxya.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3lvjmoiuw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3gczooojg.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dlzxbvzu.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dtwgdegh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iyjruonk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3egsmbsyl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tgdgkzdc.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xpvlcdlo.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xnrkqjlq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pysdhmjy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3nfrqvpmb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3vhgnpaoi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jekbkgrw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mjeajaie.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3pllxenkk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ougtxzut.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ijzqgzgt.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3hhwmuesv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3aledifvl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3mtocpilh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hrrkutjh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hgsqorqa.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ancyfcxs.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qwwggqrt.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hzlvnebh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tmhuvdin.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aywuasll.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pmhzhfvy.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3steoewis.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3unazmpzg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dwpwdopk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3uiyykutf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dyzqwzdy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fogbhjdt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3cvsfakul.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3waawfmiq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3oidpptyn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3xwvvtsdq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3szeptpyt.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iedzutmu.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3xznrdhto.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kthxptgy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3aynobcyn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3itdifcoe.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hkfcigww.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3wpflkjsj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hxbpxtfk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3cazzbuxw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bzjxajzc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3honrqzow.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3psyqizny.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yrcvdhpf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ndlkymjv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zisobvgd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cnlmekcf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zsasqskj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tfdcjgfp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gakyodqu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xpcwcsgm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ehizmfdq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3qkfkgpji.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3cjocmjyu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3abpfmlpz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3iznuwlkb.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3pdihwlda.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3gnhnxooj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3diacqcoe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xhawohur.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wvqvxaqn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3oxwpjqnn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3oxcallon.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3nbtvkpwo.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3qtnamxno.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lijkmcyn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3byqokcep.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ucdhzqnx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vjicflzm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ncjxfuuj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3qwicrvvs.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dredtnux.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vacaertc.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3afrcxsec.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3kwfgyyqm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ykxihlpl.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fhnnvifp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3kumfqbdi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ccykhdmv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3lpazjbao.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3zoabfqwr.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3hsptihxo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3qpeaotzk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qggzvdyg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3abvkmtvx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wgdwytyp.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vxaveuyo.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xqdsgmrg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yitjwqpg.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zjyyiycv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xdeoqgun.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3xcloofik.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ognhviyj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bwlmpxyo.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pnnrvarx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3clzzmzgf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3ranfgjaa.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hudyhgpo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3pzbbitrt.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nnzswxcw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qrrzvahi.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3iftjcimk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ljcdidre.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xrndoied.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hycxgrwb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3mkhkshnk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3irkbfjbn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dhipipgl.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3neoevyjb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3yghrxkog.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3uaxyuvsl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3oedabpdm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3naxeqcpz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3hhrdjrnx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3dqaorpzm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3skpglusm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3noyrukby.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozinklpy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3qejfdper.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oqryhjhm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rzpicoqm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3twfoihiz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lhquurxc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ohkumevb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3obvdxwqt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lsnufovw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qrtmaczh.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3unraohtz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3daxdibms.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3spwjahcy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xaudrrfw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3yucdbifj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3xqnjemdp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3qouymvbo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3jdfacycj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3gxzptazt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3urrhwgzz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ifgwikma.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ctlllldj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3elmsywro.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ybcnqisj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3pknilbbg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yclbtean.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fgszszcc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3fmqjultt.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wpxsvgeg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3uaiwxlxe.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3mcqbqnqn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ionxctge.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rhegidpc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3aipmwuyi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wkdtlwww.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3xdcbzrmo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3wkmdibcg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3sxbpswyf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3kfqghcmk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cxtvdgsw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lnxvzxtn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jznvbdln.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ypbceerw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gbasolna.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3iqnbwhwr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3lajsepaz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lprbtzix.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3jltlrzon.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3sfqjwkss.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3yggudxvb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cofnzxni.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ocbmzgir.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mywsaeza.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tcvpgwti.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jdccrekt.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nxfwaqvd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3yhtngbac.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3txjbxapv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3miuszmcx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3sputntcr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ayuvukrz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3qytqdrit.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vxocwtlz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ttpzfyqg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3zzjbtmoe.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3nutzqaom.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yjzhomub.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xieeklty.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3powjizdh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3uipznsth.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzsaemqd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3cqwqdjva.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3btcxasao.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ifhhpodz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3bjtvuryu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nqibzgdx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aczazvfx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3dcjcrryb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3tdgahjrt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztcnqjqa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3orhblkdw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhvqupun.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3lfxyylpm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3cliqssja.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3jvndlsqt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3sbehvytd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3wxingmda.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3tgykzexg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xqetsozb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jabwljoe.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sbpdksez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itwjykbx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3onifgcgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvjgmzam.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3avadmuge.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3pvnlipee.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxhwujyt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jtqfqhfr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fdzzvzza.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3putiirrk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3eqcijuxt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nxwsnawi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3brafchts.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3sctbiwce.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3leuciruo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ibztqhvx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vsosxvqu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ceylvnbi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3glmtorxb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mnzjznfl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3locjakuc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kwoukbuh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ysetwjei.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3hvkmtdpg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfslmvqp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukpmhmea.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3aazinnsz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3detndesp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yhszrfyk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3suwyjoct.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hbojgson.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fftjhtek.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3sjogxiyd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxaphcfc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3syxntaql.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjfpnajp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3gznlycpu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3xnwjrnow.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3jesjxezr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3fknpndxp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nydhqwyh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3vcnfimil.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3nmqewlmp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yopzssdb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3egdnamkh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgxlosku.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rhascunh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3snvogstx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3zokdqftj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ekiczmvu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3lhcdcrep.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlmgpppr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3chzqsutj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfckrbfb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfzuszzg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ghfmwafn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mhaxyvxn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrviyxbg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ijoyqrde.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3kerzdonv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lgbohmdk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yptaolte.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftwwkair.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qyjdcwfq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cabdccfu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fnkkodtx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3njlgiuxn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3govxnbfx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3vtcyxfnb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lbskjxng.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yjhuwior.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3trmlxfth.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gkzfsrxy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3swfdtmtw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3epwckdwk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zvijdoxw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3rosevpxu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3miodkafb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3glvewict.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3shxmbiur.html


<!-- 参考信息 -->