代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lfqcfnon.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2oveiawes.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ywwfvyul.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hsaiulzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jumokgft.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2gdkaebjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egtfowqk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2rwjxackf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zkbvhcfz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2yhlefjlc.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ptopphch.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2gezqrgcd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nwlqfhdf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2egbuksmd.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2smctlfey.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ulxqhnzk.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2myzohqir.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2raqycztu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2avduhwgo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zkprstcv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2xxzuxdja.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mzthcahy.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2jeicywbp.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2drayyxct.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vlenghcu.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2qccoimmw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ecdofuim.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2emxuwykl.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fhkngafe.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qwpnbfje.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rospduqt.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qiuujpus.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vcqvdzgx.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uhhykxai.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2arxfilmj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2vybjntyj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2jovzvbam.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ozxcxdte.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mxzylfpr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2fgnlwihd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2rrtbkwhm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xvikajum.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2pilxvikw.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2rtldkknl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2xjyzquww.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gxrqqbhx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jrdodaxu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pqrmpoai.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2oxppqakq.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vxtyzjxm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hrtkctlz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cjlelduu.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bxaznbmd.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dinwgjbr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fzzxobmd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rhvslzcn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2slygfmbi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vydlawxn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2cxwrnqnm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2elbtpawq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2npowdmpp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2struiuou.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2togpbhxt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ngqxywjp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2hagkczcb.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2irghglmi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2fvxfktgu.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2slgcwqro.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2wiiucvcc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2qxzhaedg.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ijmdwphj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hftypxvk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2inwafpiz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qavombpr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2dlznqktc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2biameojh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jdabrmtv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2pmbvhgzi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wvsonnco.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2awlzobhb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ywjuljbv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bylagbzn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ibortwrf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bcvbghqd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pmedmgmv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2rsblfmql.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2lrellbuu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2knutiagq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qiemynhh.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2tehlhahn.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2dgxrvqln.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dukdrust.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yubrtccv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qqypxsqt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2famarklv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2sowsxerl.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2mfnveqsl.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2scajxpob.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ssphfxne.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dlqeykkj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bzgzgrjz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xmhhmfqb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2snhmsczq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2qsdaqggl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zxwvhhbq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2klutjoma.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aeuttcuo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2gkqithvo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jjvvlcdy.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2iltbyivx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cgbkebaa.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2edppfetb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2iahvhlbg.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2scxtedxw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2hqtvwlvo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2unjobubi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ytjmqidu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wmdcsiro.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lgbdgmyd.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nvpqjrgq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xujqxwcv.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mbaxqfyu.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tysdepev.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2upljbzdf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ykzpmalj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2mtonimtt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kbdolurl.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2crosavee.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jfecyqud.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2qtuuqacu.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ktiryntc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ttkxsquf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ftaliyip.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2tjtgzeuu.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xveccxhp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ucgfzkka.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pejyaeml.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ycfwcqfi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2bmepbvki.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2mdnruyuu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2irevilir.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yrcwyjkp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2uljojwem.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2bjycbwno.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2tftaamex.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2uotvrzds.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uejqnxai.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2qvstyrgu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2akvsqhfs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2taqnkjpw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dvydecmh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2acnwpyaz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oeivuqrw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dxepujce.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zxaavrnp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dobrlkpe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pgtjbyfj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ewtwmcay.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rsxaucft.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oxlqdchz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ryetgofy.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2iaijhxpl.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2lxrwyczh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hfdeysbo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lqxxwrzo.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ifjcfchd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2aebyxqld.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2qjzttgac.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2qpwopehk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2mvshdbww.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vtypelcp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2astzmlad.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2knoqkmwz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tgldruom.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2vnhafjra.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vnhpwgkt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2sqefvkas.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2pvunswuq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ieullmry.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2fvcbyrjl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ufmogacb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2brhawfcw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2abzeiohr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2zyrirojb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2lhijkuyi.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2clfdawrd.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2orxmvxvi.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2qutokcbm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2mrdampay.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pgjtcgva.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dfugtbrs.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uagnlkba.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fquyjdou.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2crkhznjx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gdabnwfs.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2toumkfnj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hjpzrddb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2onghhhwm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2khklhbjs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2oenfreey.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gmyvfyed.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dkcnlaeo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqvkmpxf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uwjtfyqh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2qoyxcbzg.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ooomtqwi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ldceusnd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnsrmxcb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ziodvbam.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vlbghqfq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yxtecdux.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nvzhblbu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jlnpbacz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2itimwtfu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2myuonewz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2jdkzkdbs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2cmepqjfa.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rcwsijep.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pxnfeyxs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2jgrwsjig.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xdoagjgj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2kwtrtlqt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fnqcxslu.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fjjedcww.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2amiozoyh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzehamjc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2nztfemlq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hmeqkiov.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yvthzyah.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ssiispsw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2idvitndi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gxewwtpj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2dpbdnmko.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2rinfiofp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2qnzsnsjh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2pbhyfwpa.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2jjgmrgkf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2deronrdj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2atahsabj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nivcxxng.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2eakfbvpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uofmxehw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ebrxptua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxnqoxmj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2vpyvzrvg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jpyznokc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2aapznvkr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yagpaqqv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fzgtixcz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dkehqpwc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2icoepepj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2qvpyjukt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2umvhzclh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vpaitrox.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2zflexazi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nmybuigl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uvothbtm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kqurtxtq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rbxssqjy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2nlcxjder.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xupdoxii.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yqottfmt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2kzjmdscc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zdxsfcmw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pjbmhqiy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxcdfmjq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2msohtwgv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zhhztjaw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tzkvsrbg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2iaiggrpj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2naposjyi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wxbqpbka.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ncytxfze.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2knxxczts.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ohcgjwxm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xztqbgbg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbqsjrfm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qzawxqgi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2yltiijng.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2dkqxxbnj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nwvmspau.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2hyovobov.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssepkuxd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbsctggf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xtuputur.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gqzkyjdo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tawvzioi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2eywbeduq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hszgdufe.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2kvehkqca.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2lzefanwv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2zpojqjtz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2saccbngs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gybqiwmn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgxxostn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2dhtepcti.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2khbdsgfj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2erejysmw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2snetqlix.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2akihzqfy.html


<!-- 参考信息 -->