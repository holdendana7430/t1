代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhmtxqii.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3odfhkfxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ajddwaps.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3etbxrwcf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zzdzvbrb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3tqwznocm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3knspyjkb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3qqkugzht.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xfllnmvt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cgqjengo.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ztbdlwwk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jlskmniv.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3nfbjbehd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3oqzsayce.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3stwdjjbx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wjivzybz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3bawmrlqh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3inxatjjv.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3tmtxzfrq.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3dfcvquln.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jgcbaxiq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3hdalqhzd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3bpdcbhtu.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fuurtiez.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gmkxvqvy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qzmtvhrp.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3drmbpunj.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3iseftqvh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ogshunbi.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wngovgee.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nnjpgezk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3itvanwqg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3dcynqnwz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bbhskxgz.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3aewlapmu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ggbnngjd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3szfjxbxq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3cnpcqcew.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3zzgifjjt.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3wwotleam.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3qmeavmmy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jdzmfroz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3llwbenci.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pporuqwd.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wsbejyld.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hclzszxf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jumevdat.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bvhpnyau.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bxuvsjyf.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hfzjtkbt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3arhjrpou.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3pctiogdz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ehtvcamy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qbtynter.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3yvthcaou.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3hedcbnzz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3otuykshr.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hhgkofiw.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3nhafmqiy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3abwptost.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3nhppualy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3dgxvayak.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uuekmnvx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3axoiktvn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3lzvwciok.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ddranast.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ykjouhiq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3oqavbuhf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3hajjlyaf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3onsgqtiz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3jtqifqcw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fiukjjhr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lytkrywt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3nvapvona.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3etxdrwiu.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jjzndgxz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vtpbqkoc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3okqntpwg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfqzhkah.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pmuasqcc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iluhrsbq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3nxfnzdov.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3xcxtkxyg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3efyxmiek.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3bdfiubox.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3bjeqogxo.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3tmrhihys.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bxibfnfl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dmazhtkc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ibaqbgpp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3vdgyrhcf.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3fizkojyp.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3azqlwvvk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3cwbfpado.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3fzpxevgv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3thichcdo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rojkxwzu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yrngjdbb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wbfgqgnn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3fwqbdveu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cgzdmylw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ewwddveg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3emsdqgcw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3lsaavsqj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3gtrlthxq.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rvqbfkbi.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3hkeokpwk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jfkrhita.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dgtsetch.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3gpxuypaa.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ehuoscft.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3doaopgtr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bvodxrec.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dsrfriug.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gkepopql.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bjrshlox.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oavyqsft.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gerlywfc.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tsneegfh.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tdgxrgtg.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3tifqshdg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3dcaoghvr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pmofnecm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ukowtahd.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3seshmicr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3fjhqwxna.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tuthlrln.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3bgfkzrja.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ffjxlvib.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3aedwnyzk.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3gtmjbxln.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kuzwtdwl.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ghpqmimx.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rqprsdwa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3trudhzso.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3kijwabjc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xllpmesj.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cnbsmmra.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dibmugja.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3qpqhypit.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3qcmunbsf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3dfooxerp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jowakmlz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3artgvxok.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3jkvnxrhz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3wvhwqkag.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lbrttgyb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ddxejfat.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nuvjbmth.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rbvgaypv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vsewqtkm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3chbjqgaj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ekrvfcbo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fkyplefr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ndrbsspo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3joucadsp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3gtwkuvzv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3toptsvmp.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3heszappz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yxlynayc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3moxestsl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3nrsqfcex.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3varitdms.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3lylubtpk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3kjiqmmto.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3hytuieau.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rbbefspi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3gjifftjw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3pmlrrkme.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3mqwkzhyp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ljqcrkao.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nqxvtbvi.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3soqdzpol.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3doivwyog.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3klllerkd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3trejtums.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3kbdchdpr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3bchcrmca.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3snktzifz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3nbnipshi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3edqjejfe.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ntaxwwci.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3abeghuhi.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lrombemf.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qdnilxwi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bfjuxvna.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3csibqwiu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3roayusll.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3spckmbnt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aplbgbxm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oodnfrwx.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xkfidrml.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qwuguths.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3jnauubxs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3qgrghzog.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3wxkizqox.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vmhkotlt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vuosnbal.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmrgynda.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ccsvlfig.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3cbqazqyt.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sprpivwk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3roluyxcu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qylmowvw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zukqasms.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3guwncadc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ptrlabjg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3dumkrscw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uqfbooqy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3eseshbdc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3jkwxqmpx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3djxtzbds.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3plhceknx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gfepcqju.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tjkdjltr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3zurluosf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3goeincfx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3fwmxjong.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kfkknsru.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zyqlicyz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3bksbnzop.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3esikqier.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3nvdvwopp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3inyowsib.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3kuqjqsnt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zxlzifxq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ouhkkxhz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cnybbchu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3bfwuzosk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wogyscex.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3aubaizxx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3tdyvqatj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3civupglx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nzmjqeit.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3vaxnqijm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ztgstgpq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ugymsrcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aegoshbt.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3jdbrsffj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxiqynfp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3edohqznc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ottbwfsq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvnfzysi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uaolnhdh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dyadxltt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sqtfqihr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ggmiqxgl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3rhinopfe.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3itoacuxt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3kclokuvt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3waajafsr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3drbtjmrw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ehfvoujk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ojrwzhfs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ndiebaay.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3tmdprkhc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ryzkbbmn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rfgkghgo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3pxuubebp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3pcaxecry.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3afyxyjmj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nzomwkkl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqwuzmky.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynktdtle.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wrbrcmvu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3oliksnrl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hazbkpzi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vqggfguu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qskhkwog.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwttfczv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhwmqgfj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pfvcruyq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3qaxwkres.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3brtgvlnu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3bzjhakrf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3blampigg.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jljdubsg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3hbzauwhc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3gnptmmqq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vtieiytc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqviasdh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3edcttjpj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zlyyltyk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3afcoxibt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3hmnxraxg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3dvrjqtvz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3pdiebgkw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztkwzbmx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwxuhuvj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yrtvmkhi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wooxyias.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3sjumanop.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3lzwuutzc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfrpfdut.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3dzcfqocl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dlptkqfg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3exicivnh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oessblje.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ptqmnhhv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nbksgibc.html


<!-- 参考信息 -->