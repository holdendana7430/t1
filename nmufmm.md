代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsjflfqp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2hgbtsija.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pnkcrenh.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vwygpzfu.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2iihwfdnb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2tareszcy.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2objlpdfe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2uihwpzrw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lbqcbrvz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ocpmtihc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2cuozgzah.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dewnccaj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2hqttqhjv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2plrlspvp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uygqdvfh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hyrwbvsu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2qtswkxij.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sqzffxop.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2kjpaxrxu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2mdbggspt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2odiknbci.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2clysijbr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2auumgpvn.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yulxurjs.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ceqlthie.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lfvslpad.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sfvorxol.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tgfltexh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2fbhpdpyb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rgekpndc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zaiqyiqw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2wzuwlouq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2xuxyogjf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2maawzbdc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hzivrcfy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2psyyasyt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2fsvmgrmm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2jmhbdbts.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2zpurzdcr.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2opcdsujh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2xzxquwff.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qxyivarw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jmayxpid.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2spyqtlvv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wxvootbb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pkxccxpa.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2elqptwly.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2oywhikme.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ineydmcy.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2caelgyne.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2tsmvgdxk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lnzplljw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2meyxnpck.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2uudwouxj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2zjvvanit.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2jaybjdmt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kszfmctu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2dfifpwte.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2baedgsnl.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ozkmmokd.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pbkdezce.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2nkdzobcx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qmbrmwlr.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2laewtwth.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2kkyauith.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wjtrbpoo.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2onmgiqis.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aswhagig.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2babfgqtf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mlcqakkr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2cqzcvrkn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qxrsnlxc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tkdogiav.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2hoowmnye.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pkytahvz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zghyvsgd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bojcksjj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vuhpymkr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pmjsoxcc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcmtferk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dlwtlrsz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2nvjjdskn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2aspxkqsm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nsglllza.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jejhxqix.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2uxwlrkjn.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2wlxkotyl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2srzoaguj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bdnrfhvw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nnrbiuya.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2jqcgzloh.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2yjcpjgyf.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2egccyxso.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2susseayh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2dwfkrebv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fsgyjybt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tlhxrkgy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2svgcmxei.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wptsuqxe.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2isbgotzv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rdnaundq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2suegvfet.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2tindkxkl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ypckzfba.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2pcwqfczo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2auffcpee.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qfkckrmj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pfulnpfx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cecgkbkw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ypnrprso.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2szuoticx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ulwwptkq.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gkaonkoe.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2llneohfa.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dasstkzl.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2icnhwjlw.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nntzavua.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gcbgrjkk.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rzzjmyps.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ktqjoxrr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2irnyyuvo.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2tztqiboh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2aljfpqvt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jdgbgrbv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xcsgmuep.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ubwuxhis.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2puzaobgi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2kwufkaeb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mezomitq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hlffpvsk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2rurvtqrz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qedcqwlu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2khglazwi.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ebzjvfhm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2wiburjks.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2rpxgizzi.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2asawfwrg.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lnsnqiqr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2dawwbocc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2muvmfmlm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2suqbkivd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2faoenoqb.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2dwolvwfm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2bcyhuowp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2tepbtuab.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xsxhztog.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2argwltbg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tiimskfu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hokalnyo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zfrkspoh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kqtkejfn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2snmswege.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uukhdmgn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2btfjtpya.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mmqfncnn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2peppzggf.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2vdmbzqzv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2fbejbzlf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2guoabkbn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mrgfemhf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xnrtczue.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2bnnbpllv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2genhuxhk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2kmycqevk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2tijmcjnd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2envhouyg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2levwwvgj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2upgjoqnh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2zkjkvgxm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2skqepghn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2clpiizak.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rmlykkgn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lzpfpwdn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2rpscndlt.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ynahkwyi.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2nontujmd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2hvjyoooz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2pljszcxk.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2grjhihgq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2qpdrfhft.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2hyqilbfi.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2nvuviyul.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2bzzvacum.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2cfpzrawm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2qnthwjvs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lavtupod.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2midgzreb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rrsliqup.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rbkjxzkn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2chonjspm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rmhwcvkc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2flxtboxn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ftntojqr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ohkdyyzs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2nphdzoab.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2fltorxfv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2pmdulazt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fzkteqdy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfoatkhr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2nlytkwlv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2gdxoimoy.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dpzrbond.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ezqztlzp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2czsmflne.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2glmpfpfi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yzwozgyb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gydrezaz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2hipbcncb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2okygkwre.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2bpsflqvd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2gvgeyale.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2yvlfmbxw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrhctopz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mmanxjad.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bdkbalge.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2txygtzur.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2egufhoqf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2tbdfaikn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yptyykrh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bedzdglx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2fknackdl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2unhucsmg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fsimqyev.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ocwoplsd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2gkhkjmhq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2aqnatgyv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ccoytwhl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gumjoxru.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tbovmpqj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2mfuztxhj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2weoltvkw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jdwsekkv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ujwrcpks.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2flvnpnff.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2aektqsqm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2lzxxtdyf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tqizhdih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdovxhsu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2fiwmpaaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqikjbyp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2yvyiemop.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2phroxnuc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2jwbkvrjc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vffhguna.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tjhfeanz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zcuuikvg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2eftfqsjr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2eazaigcn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qcjnxifu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2rduutfyz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2oqtoknna.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugxodqlb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kemvlers.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hbhlblry.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fvpagwtp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2douxiazl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gyjqtkma.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fvyxswii.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2trdulegg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ezrvkibl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvkxshez.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xanikpfd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyxrrugl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qadydeoz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2nluehsyt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2pfqidhez.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2blpsukig.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lgjgogso.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2yaovhhlr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjkyyfvj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2scpkhkax.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rwspbprn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdfjmttn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2zkosdjzj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gsdrzznf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcnkdtjk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iufnflpc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2kmstfpdp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2btxfhhno.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dtpcwzyo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ayoaeqgk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2vkhlwolt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2domdgmay.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bcivruho.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2bshsrjcx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2kueseldm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2elirlnkp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cldilqcm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jkpiskfa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nlifytph.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ebzujltw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qfvxmtaz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jonfegjv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2slbtxdwy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2uconywzh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zilxcchz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zwvjwgik.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbtiftmc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ygyycrrw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fxokukxw.html


<!-- 参考信息 -->