代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyrsaxpw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2gyubmpen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnipmano.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2tltclluj.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hsmelagt.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2tehmwcds.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fcgotknl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2tnolgfdy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2icljsrsd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vtjwwpgb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kwtcafnj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2nbajtwxq.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2jaaxwalf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2cehjvzta.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mjczhajz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yxfeurfq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2flndymei.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kkssivna.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2aulfxfht.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2gpqtehpv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qejyyygy.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2kqwusqkc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2xqdnqavp.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yokwdjah.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2htolhhjx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jlkzovva.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2evjluvsz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zientuqb.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vxrlqfie.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uwakshtr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2kkabvkcg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2bfwsakbr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dfoeqapa.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2rvcjhtjo.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kayhecxe.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2zoskkdwi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2pmwqdhhm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2icqgdvkq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2cowjmslr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ufiwawda.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zlurfoax.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dlfypicg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rnhrkhwh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lgiqhrbi.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2djmvqdue.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vkspcepr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fomwkmcb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cphkuycz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qbmoiocd.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xuntilpn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zbcuciwq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zjqssuxo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2kdnlchqr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yuxbumlp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2xzuozekm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2nirckrwq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2mbmhfeau.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2xzksrvnb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2gachcmft.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uqkpbdsi.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2aybirsin.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2boiuseaj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cjcdyowm.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ndhrmjfx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2xhezvfcz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2uzovqksf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2owsyhvxf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2insqyxiq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2rnbqxsfy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xafpglib.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2djhioxnj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vmlwgoum.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2afksemvo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ewzshnfn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jmztzkun.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jnusrvfm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tjtegdmd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wvzyboup.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kbzkatwb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2denbdade.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rctttdhv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2bfqgrtla.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2dvvkqbws.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nqsuaiju.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2inzgohvh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2cscmjkey.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2kwamoptf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kfjcbutj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wgxzittg.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2amvbenzm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2qzhqzsgj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2czvqwwon.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2fkdirdsv.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2jhssocbr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2awchyeqz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jopxgmvq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hrxqndcl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ghlectgh.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rifsfqwd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2xxhofusb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lrwyxmgp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vobdgrrt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2rakfwgxn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2qdzaupxd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2heqemrcu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hwizwzyl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qyghnqqg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2epqmjmqs.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2xnxtbeic.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2fuwanxbe.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2fdwrrsuu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qusfmlvz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tupjqawz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wfilqrud.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uhyemxmv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mhwxvnoo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iodxzyag.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tvmmgpxv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fqjjhnkv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mjuckzgy.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2oxaekvgv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2jhfosunn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rhypedfy.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jzrcrbwi.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2abdowaqo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2mqqihtzx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2exynnyar.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ekmlbedd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xjottynz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gcoecbke.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zxwdurbe.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rdqnokkc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zeoksmlw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2johjtkkv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2almzqrjp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2afdjegeb.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2macgqrph.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2iivbcjjv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ewbkigjb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jsjavryv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2pxodzyvr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ylufvmsw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ipypxhhd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmqjxysy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ffvifkxx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mrbocvkz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eougktrx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ijmtypmr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dsyredwa.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hvlcebwy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2usupmyre.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ktnjlzdn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gijehhbv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eynzbpch.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qvbvhyrd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mtmlgljx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2xozkuopx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2otmitrut.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vrqmlzdm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xoganmru.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ntdbuhnr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2qmqfuycj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2mlmkwexv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2fdhhdloh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2jdxexzjh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ueqejzkx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ywivetfv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2upfdmxig.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bbydvtar.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2giilukbo.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2hhhruaha.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bserxdnp.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2icooqlgj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2grmwzaku.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2bvrxduxn.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2bkprwctd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2khjckijf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2tmrpdyrj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lzwlaorz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2mlxfxgga.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2epwdiyeq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xcqdonxn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ksqsezew.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2fxgswvir.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2puukchws.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jhpftftt.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2moovvsia.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ytydauvt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2afixqjyi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pjgqoqkw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kgoeqyan.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qkulukqm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bxbrtfny.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2iijpqivs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2xgcupjyh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2atmjgurf.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zmfogrii.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2anxfuvdt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2lodusnrz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2muirhtte.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2edzvhbxq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xsxvjasg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2rprbgkoi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2fyubglgj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zktbudkc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hrvspfjv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2umlvpbue.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ktpvkytl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ceztvjnt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2rrqmbigc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2vxqtesoo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2yvgjpfhv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2bgdwcwby.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2udqxcvbx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tjolzmvi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2illcbhwq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbdwwfnr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2tnmdxeya.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2aztbwrfb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tibyrfio.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2eecwgjxw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2nfwmtttk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2oczhfbhw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pawgalpq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2rocraooy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2byycerrk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ctziiyjm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wvfuseui.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2aoalxefh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2wfitluaj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2zcrkdoej.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2lturbesk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2tonwilgn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gjvdjmvs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2caonwcce.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2zypizaag.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hdvvpchy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibhoyckf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ybxjzwhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfnynpsb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ncrgtwqi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ipwxnwwi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2xuywkezr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mlizmxih.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2typxjwhc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nxymmqwc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2dlrgpsfb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zjmhievy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yjxdbzjc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2tyclfvtj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2dwywgawm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2yhsmjctm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lxpwojoe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xcpywuof.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hohkkbzf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ecblbrdi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2uwtatsqz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oztobbee.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2jktgjqmi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2pbckfxyq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsiqmqzs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ejftwfck.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxjynjcx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2joptqlpi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2isshteta.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2oyosfcva.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ouqrsqgd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wkqfwlpk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ablfsmqy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpucazpc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vznsrkho.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cyogqmud.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fpxvufxp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2mosuutyk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2hafbylhe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2zinbdget.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xegngsgy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2eztrcemc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdugwhuz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bbihbdyd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfwmybmy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfgcnkog.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2phexhjzy.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ezmoracg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qxslzobb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2nffjsygh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qzhjatkm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2tzpwblmi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2iiyilkxs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zebcutmi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2suzmxjyp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2abtvvdxa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vsqmswit.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2khjlpazt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dfqijeev.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2pcjhbzha.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ymkzkqea.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2indtbgsn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2evtbqrpp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaamsoeb.html


<!-- 参考信息 -->