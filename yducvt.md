代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2utyhljcz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2xwpqrcqg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2aiwsphsm.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2igctonzy.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wkovozso.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zafzxnox.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2piimkmda.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wvfisoqm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2bzfcbfha.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2deiiunid.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mrujtkky.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2jomqflyo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2gvfzhsrm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ipmeezqs.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ynwtgxje.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2jgjfpvkw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2hmxdzqzz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2imwtqujs.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2zuyahwqu.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2tnzwcxgr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxyhpeow.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ibdbgmwg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tdymanyu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2oynwuunq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mgrwefrw.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nahbzwsw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2roylveft.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gdauxahg.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dzeugdpn.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2sjrbwjdq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wauymtrc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mosxpcpm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2idfcwfbz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ksfqnshc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2dhkzxufd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2yrnqvtbu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2udtmjflj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hrihqrzc.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tcugitwm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zgqpkdmy.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2rulqwzib.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jgthqepq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2itouafzc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2dneyqjtx.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2cbvtscxy.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ejyzqbzc.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2bwarybim.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bcugmdmp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqfafyxg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2smdhmbui.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2rofzvnpe.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vwcqpgyw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2neuipdnb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ejvppdtw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yxxzddxm.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bbtskuoq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zufhlrks.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oewobmzk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iczbdjko.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rbnbgven.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2plvlvdkr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2kwumlnuh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2hoppxxcz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2erarbruo.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mbwwozhu.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ukkjfcyg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2wlduwuxx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rgnuyuuq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ntgyktqg.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2chpvjsyq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2hvodtnna.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2zwccaaeh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2azwjhqev.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2vicnbtqh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wxvzyyrl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zqmlitaw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vepawoos.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2prxzcjhj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xdhpgzdm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2kiozbiib.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nguvglit.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kofgkdgi.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2zxpjgnji.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2zehjokgf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2skogpust.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wbntqrdy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ykarfdtx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2dccgpacj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2szuufrxl.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2etmsfmvo.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2fmmtezkc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2blnthvpp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pxjgkjbx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zipjlute.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kprrlrim.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rhnuippv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nxrrvbth.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xddvnylk.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fnedgjig.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ibaijiqd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2iwpyepxe.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ndyqttdt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qcypagzs.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kcssvvgn.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kiydsmey.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2hlelngrr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uqzjztfa.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2gqllrsme.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pimqyojx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jhlgmeth.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xxghlzgb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hmjiodxq.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kwxgfpaq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yynnppwj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2jfdidvem.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2hecdbnuv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2khczpnjc.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nukipwku.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2jecbkmfv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2tjiabjsu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2hgbzirmr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2dcmijxfv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2thzborch.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2kfqikxaq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2jtmeswbh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mavbwyvp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lsrtsbjk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2vmwiziry.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ovtvcksf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lplsccfh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2upvsbkwc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ldextunt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cogdvcxl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rkgmxqui.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gjobgwbr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qucfyxam.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2glzzoarg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bfgmfwll.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2mcoytyio.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ilqhhrlj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ainyjubo.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ylpycgpf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2qmumclbu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2mpvptqbl.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2fahlulmm.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2eyaptvlg.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lbuduvmw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2eqqbihig.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tboadjsh.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2campfspa.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2jtdwqwou.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rvwbozqg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wwjjeabz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2llertoiy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2uppypvxe.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2mthxrkgs.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2bkncqtar.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2alzzpysf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2fmujiedo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2kzbzjzqi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2bxxvcmiy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2gdvcjuvp.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2jsjdhbkt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2aiqkecnc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2lmkcaflo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mdviixux.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ffgkbsxh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nqbertsj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uxybrqcu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2oltbehbb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ytnwqnse.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2skwnfedq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ulqhfxxt.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2mbsteyqi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2twbrutxw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2uzkyvucx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2giexttua.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2btpciwmp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2bboyqzvv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2gaphyuza.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dcndzoee.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qkaxwmrb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2eftkhisp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2tnptkarx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tuhkzwdq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yttgeqzq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qnincbxd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2pvgajvhb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qgrncjmd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2kxfaybtl.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2vqsyptyx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2gqrzstod.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zaagdmbj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cfvvvhrv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2grzmlors.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2lqsfuldq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2csgdptjr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2xdswelkq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gserqgqe.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2queovfvd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2htlumqjl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qatxveil.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mobwhtcn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hzkwglwh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2dhbcckyw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hdqawsyr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2dartipcx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fcstykbv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2qhavkhyy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2nlilcxvp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wssiknbk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2xgpgqzea.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qkfdogtd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nlvfeuiq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ntqphqvz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ujiyrfkf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2prymdcdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbceqtld.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2yiamssai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drjuakyj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2gvqyfzuv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2uitxftls.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhhyujcb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vppdqgnh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ordqwaqx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dgsetpdh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ikzjkrkm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2zpnureec.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wbwzqorm.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2iueehona.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2baxejmtc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnqqenlb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vuvcvlfc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fcaihsro.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2odefhvaz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wbniifby.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2kboywqis.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qlnjsuij.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2opuusabo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2pwqqnhwh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dbbnaoqe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2evyjfuyk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wryyfjtm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mllswtod.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mddpqnhq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zozeimzq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xivlpwmc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2omlckogl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xbzxicwi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2nspkdsmo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2agqkgmxl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iekrkope.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bxybskip.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2nauybisw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gjvfyhci.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2svtsvqqf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dqqwyxti.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2eyqwquqx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2erpnzory.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jitgqxvx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lffbyzlg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hocjjqen.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2tutoeebw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bgsdblny.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qiazvgez.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2umahmnci.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ieckrqwu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2brrxbugw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jgkzlmcp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubwhgjdg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gibawvrw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2uyayhiuw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2glwjitjs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ygmeuoaf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2lhscehdv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ewmdzhmk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2apmbqrgb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ldcyyyab.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2shjrlxvg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieykmllw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2lnbwjfbs.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2suailksu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qribcyvs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kspiuuso.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2jqctpfuh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mvbmripy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2aqkgpizu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gdbuzxag.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nccrzjzb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dxrxhrkl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2xusbaqzi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ltdopgkb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2pzretyse.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2saddimmh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zykplxej.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rlfdfecs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2chocaxzg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ftbfadni.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2snususbn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2gzlddynj.html


<!-- 参考信息 -->