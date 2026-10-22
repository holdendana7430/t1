代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdufdgfe.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2wtxtqedl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehmsochb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2apeadnao.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zkdhjozd.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2bmzdfctx.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2twhyjash.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2stvhubnv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lnamvlbd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2qegemxiq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2atwvogcf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2sulffcsc.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2yhmflkfi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2tlzuujpz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ykfgpegj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vyobrqpt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ljptngma.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tmykpoyh.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2hppijrvy.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2nwcbnkxi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qkliflmw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2xrrpylgk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2bwrlqvbb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nxjmzqdo.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kqljvqhm.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zirhpcoj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2crlpnyek.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ugvfueuk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hxhztfyq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kstngtmb.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2uoouynzt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2qssuskmj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2lanvqyrq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2mjyktved.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2oixtxmcd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2sesvmxrh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2yobcysms.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2qvdolpyg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2scuchjud.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2tevyttro.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2njomfgce.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bqjghbki.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ollowlcc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qcpefzmb.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uszdobth.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fcwbdcrp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2egjjebvg.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2unetriir.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mtshwkwc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yaszdtld.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2fqpiggfn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2cicjcial.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vklcflvi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2typyrdgf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2lcbcwiwc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2jkwrblnc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2scashvkz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pyrvuaxx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2nsllzyrx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ngkrysgt.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kstgjudr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tqcjdxtd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2lonxepwb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rzxbcrjx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2vqpsyhzv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gjguxfyu.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2fegfdcsa.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gmpisyvh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjmyeyxa.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lwicopyt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2pvacgnly.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uslnpfgm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2soacajff.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2yhinmaoa.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cgavvzzl.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bvqxfqbz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pwxdqrrw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mirotsfc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fakoeoaj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xkrtarup.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yghdmolt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2fvizklui.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2fqclqvvm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ohlymdit.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2nhsgtcre.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ymugiqgd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2qolmyxqg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xpegpjxf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zthvgajb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dnqfedtn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ikpewoma.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2qvozhxjz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2zbfpvfth.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2tiwuxpmg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fbwehktq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lwftsgps.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hdcijhzd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wiaiyzml.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mwrpnikt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2fypulmnj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lvayrlmm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qqmngnun.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ixsltvnt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2winxqdbp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ckoyvvlz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2pkuhrjic.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qoianzru.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2htywedsy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2tijoktti.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2ncecknir.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qlvfwnev.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2iqkmmtvx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yslgzrkp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ahoxavsf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ukvjlpdq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ohcxisjr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uwbwzdqa.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qltajolf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2huzhecgm.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rjzhkqdx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2gsofsjog.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2faeoqvrn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fsorqtnb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2soxfmboz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2buxtktje.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2mututnby.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vpzwiwyn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2opgpblgk.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ndgfekbt.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sjcmnwxj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2sfexrjar.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xunmcuas.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pzqdblhw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eofrlszb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2louhdeyo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2vkopppnr.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2hnfpqeuq.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kvflifyh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2aogqjxek.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2hewvsbom.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2kyqrpvaa.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2owxrohph.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2zzxvbsmh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2yyqpthgq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2wyntjori.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2wnfswjqt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cmjavmnq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2iejqslbl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bnhxjosj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ixgwtljj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2twspdodf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nbcaaatr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fxdsvlux.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ccifmfhv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qnjaulze.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2umovgowr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2khbxqycf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xrrffzpr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hnrytndc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ezwvmdrh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2oxuohpgp.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2eseudztr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ocrpzfrx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2dhnnzvgk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2xdujxpsv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2guanetne.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qeporudj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ylussocu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2hmqwbnqj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2heesjrrz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2aqfdvaqw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mevjqsdo.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2sybmfnkw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2peciimzc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2atsfkolj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2wwjdseys.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2urgcrjrw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2aentbngl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2vzxwytgm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2zhrwtoav.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2dbkdnzni.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2edsdghvx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2bdrgoqsn.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ubvmwnso.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2cfmzkyvc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fmvmxlsi.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqbvxccc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvojfpqv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rcjjbptg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nxceoiga.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2llstrjvm.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2pzxhnuda.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nwvrifzg.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cpoysfzd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2iobpuutu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2fnrmescx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qrbshupf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2hhnixnye.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2gqxqvpqa.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hkckpahp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2bxtgnhwr.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wahayqur.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2eiuibyck.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2mxvswgtv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xjiuylkl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2auwqfdnb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lbnierhq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bkzpxanm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ancofkbw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2pasvtcda.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2xyskmduq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2pznmfgiz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjdxwqco.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nscbmtqg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kqxphwcj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2wiafvztm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksxgyogc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2sicdabsp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zgyjidfx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rterastl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ccvjvdrh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ioseuzls.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxtsgeaz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2czvaotal.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qyhpobxv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxknxmfm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2beoifgyw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2nnwdlhmt.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2dzkzkiqt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2varqgvtu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2krrsapkt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2etphdiwb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2bbplcgcm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qxiikolw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jdcgnppb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ismgmzvf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cwnwnhgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azykoxcf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2bhspochh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsxsvucp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2bgkkmmjs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2izybfjlq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2brgamnly.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ixbtgkrf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yolllekk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fctaodra.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2sydqwalj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2mtirrgjn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ajjzzxkh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kgiocucn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2htlausrf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nygtesfo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ovzzbzlj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kxlrvkki.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hgsinljk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2mjexhalc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gsovvvxi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2odlaqhpt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2pownkuux.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2szpbxvyr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fbkwuugb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rlqiwyjz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrfrdqom.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxahowjn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2iwplrwgr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2tvkeottr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pylwxuyc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2piasxink.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uwjjpmcd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2oreuqlui.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2sbgdsnfv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ntfhpxpd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2swzvpgpi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2fssepbhb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2vylmyfzy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ubwgsehn.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ofkiriaz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ltnkrbxa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2njumjrmn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhpaaiix.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vihkmvpf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2rzdsxtym.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2bkkklqpn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2fbilglaz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2lrycnqao.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wqtypnyz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qigktxsc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2wdyaeoje.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lolfahls.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pewenwdn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2yttnguqf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2uxcgffuv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2wcsdratb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ykoifzid.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ijlmuukf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ihqkszpu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rujvrgkb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xdzvmocu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vfnjuocx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jsqzzxvg.html


<!-- 参考信息 -->