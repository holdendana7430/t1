代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3dqsbqytf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3qouhzxfi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mezyrfov.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jbensdil.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qhydijvf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yalmfoqx.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3zynotwmy.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3fiyxcxcg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lrhgzvsm.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3dyvzvekf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3lwxzprjj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xzpjmwll.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mzufxczt.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rzkcoozj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3loadsutr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kvwgkriz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cjmnjwko.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xmwcwiwu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3spbrggcl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3oludoefj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jdprdfev.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qvcwbvyo.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3geacapdh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ankoqrxs.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3yqyovhan.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3quhgvinh.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3dfsstrdr.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3hkvjnqmx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3jcowbhny.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qfsvuixa.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cqcfriuw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vapuifvu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ohrzodiw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gubsotag.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ebcfykkc.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oyhyijir.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lktljjbm.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nycouwnu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3pzvbrqds.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fjkomiwc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gplznhad.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3snsmtwmq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3hxktvwoz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3zuvbhyab.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3sexoaxkw.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xewxlavx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3oolnrgio.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rkjxjeso.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3scegfrlo.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3onmwkoje.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mepkfvmw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3iparqicd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3dulvixdk.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3nzbzxnbx.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3mycynzhi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xsoepert.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ynjnmkxj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jpiuylnx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3hrxhpyrn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lcxomyhr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zkhdrusb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ipnbipma.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3oizoggir.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vetiqltn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lxijngld.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bmnfllgv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hsnuhtmq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3spvgpqrf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hjotwzsl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3aeiyjdkz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3vahsrocp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wahovjxt.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3znmvtbnn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3usnfmusj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3aewbhvsy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xzrqhppz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kvrlehcg.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pnknzehp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ljdsmxyo.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qwytidnu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3hkyuowae.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3lxwdpsrr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iqznyygc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3epqpuypl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pweyhjuu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dqixkmwa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ntjgoaxl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3jprvxcsm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zcthafve.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eaeretqb.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3zbfwippu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3hlgseyft.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3odfgskey.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ialpclta.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lgdqoqig.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3osrjkizl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xbvcklrm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zhxuuptc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3tlorgexg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3mbnbiqjg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3grzquivy.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3enuzeihx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3emfxltsz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xkimqxuf.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bzpejmzt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oqevinol.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jdsleeai.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zyjebyle.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3byqibedk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3jninmtkg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3clrtnuye.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lzvraraa.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cfcfsxhe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3ghvitjms.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vwtzsukw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ojvrqszr.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lnkvhngs.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3nknbpewz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3leljqojg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mtilpulx.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uekrwfbz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fgrxcfgp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ljzcqwzz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3nqwsjtyd.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ngdcyjwg.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3byfwksce.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3qbtlatjn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3epylzkmu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3uwrcephq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3fwkatcta.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3mhtdvlqn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytrfsubq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3dnmfuicv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3nznjxrbd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wcvsexyt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3crgqahve.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xksihgbf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xrpufzjt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ufqpqidc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzeorzhb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ehfiqzik.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pvvcmbty.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ryxtipwt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3djobpzks.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3bqdsgord.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3fdhjpcrm.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pabdeuth.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3navnxanp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mcjrttet.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3cwiuivwy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3pxmcrerw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3qbpjrejk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3uuohrdaj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3kgbostlf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3czdhxbkt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3kfqkspgr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3butwutrm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3udbgccbc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3fqqwwmgr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ndmulhdk.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ejeqkrqm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ruxhughy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3pccxspdw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3tiulchlu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3mxfkixtd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3iwehsnyl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3hfeuqzqo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3bhehoppc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3lcdlumto.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qaztqvtu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3qrzqcucj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3kwoczhfk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ywctyqhu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wkasnjho.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zzuedtms.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vrqwsttf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zagzaqgn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3shkpfbox.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3eywglfpc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ocggeeyy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fkahwfaj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3htkantwa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ldtryvhu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3pkepbfaz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fybcjrxq.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zvmpkjih.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3dccewdoy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3rfhnznwu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mxgydypy.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vuuknjrh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vhwnxacy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3mvrijzmh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xdanvifz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3albowbrp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dvaowzqf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3cwjcvwfv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3kxufqmlu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3rrklujtw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ootvqmib.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3hvqleiaz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3eehnwsqn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uswvocvp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zbhjanav.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3zulzvccu.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3expqgkrz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3iquxdwxq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3etrnjjmz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nwifxspr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ijvqinjd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3sirvpkrd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvdiyebo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3gldhfvbq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hokhmheq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bimyzvoz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3kbqjbgho.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3anrferss.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3fzxlewdn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3lyixowrh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3bfvlzmpy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3crxyvyyo.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ttiosbwn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hcsgorsl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3lxfrsynl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3agkrjwun.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bdaaaozw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfnolyfe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3zqairnlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjkeywlp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3qfejlxbb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fldiapqf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgnapsyp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ueblcnsq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3umtmruty.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cwrkhgio.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3iapurpxw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3fuwslnih.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wmdffvim.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3nuwrndcy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3zmtelfhz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3vpxttkkh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lykxbbmv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3taxiwzog.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jzcaptdw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3gtvxloxu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3gxwwerqj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pwvyhfnt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3kjrnqfur.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xronublv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3njlfqebn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhivuuki.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ipnzfolh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rlwwudyd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qsbvugod.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hhfepwml.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3muxpsujs.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mshwahma.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ykycabct.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcdiqozg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3afnprvxd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ldbycdlt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3cqpcyeil.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3gjyjkiui.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hkusncjg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3zdqumwae.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ngdommko.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ppbysmok.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xxccujjz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jqrqtlmp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnufdbbg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzyhosgg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3neaplwgj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3rcxyfzjc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3liabqram.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3fpefbwdr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zjfpanhc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3vcvuaphk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwjqcqhv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lyseyqpn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3crntmjyp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3vcliiomd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3byjdyoka.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3spybgqpf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zfeiyhaf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jeghpfrf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3tasverce.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qztgdowv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmrjizuv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxwmgtjv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3mtffqodm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3dixqmelk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fptnijnp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3tnvpqhrk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ytxeiobz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3movjadej.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gezkhfkw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ywfvooic.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ooahrctq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tpukdufe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ctatnast.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xlxmiopm.html


<!-- 参考信息 -->