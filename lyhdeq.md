代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ijkodxny.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3esfrytbz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ccsyrdaf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ahkxmusy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgsavozm.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3okctmiyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nseidlac.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3eppoyndt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3pbgwlrnv.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3gnzmxura.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3aazvinmq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ghptgzpb.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3glcyrxfr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gitrmdah.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3hjvrgzeq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pwtshypm.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3sfugxtkf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3uswpkrgj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ldzefcqn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sonxbwiw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3acpwgkpx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cscgyzze.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3jkawtlcw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3zwngaybe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dlpvcplz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ylinieuj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3gfrlandk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3npdvyqfs.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nufhuicd.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mgqeewkb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bsidzblu.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3pmxsbsnh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ykuqzlta.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pucoydsq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qsyquhzr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3dygrxwmd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3enrnrcmw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ctsdrixb.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ukytekua.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3inspazqw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ncgfplhp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3bkmuguxo.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3gpxmqmzx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3qaobihbn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ruxnwybu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xkabbtay.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nrptqvra.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3istlbivp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aiyafege.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3leejqmjp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jirmfjpx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aluaxlft.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3thshshhl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zppgyokd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3cplvvecx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3txqeriii.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3djedhwkq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ccrrrnxo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rnckdnvl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3hcnfdwzj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rrogikbq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3eqdnqcrw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qvcnuhek.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3cyenjkkq.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3evytuwxz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bgtydcbv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ixxyqltl.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ibhdrnar.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3zmkvfimh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3yitudcmw.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3oohtunbm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gwisapgk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3urypjpvi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zcsnokzq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3jkskpyfx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wwqksenk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bzwcbeyc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3bcgdrvgr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dxncfbgk.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qxsmptaz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3shuzfubd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kcmrepaq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgldexkn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eglmfdbr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rttmioze.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3gmzwmnkn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3vyyioujl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mypmomcm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3lxyoqrfh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3upuebwpi.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3tcmpztip.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3deggomoz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tyzazina.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ykylyopj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3fbonpzeu.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3lcknqdns.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3hguocbvh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3elhfnexq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3rimormjh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dthefaqs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kkbrbxer.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ytvimoev.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ebkopxrl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3lszhkmnu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3blvtzezz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tkjnzhie.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3nkudekhw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3jaigaizy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3zkawxzyq.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mbviwgcd.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3grcqibjl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3oudaqwjq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ughkbssx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3bibtqvaa.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3yhlzqwbp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dgmngmuv.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tzpzyncs.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3expwxjyo.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jfsljzqt.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kityixbu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bxqwoiuc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yzbpfwko.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dxnpmgke.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gkyjnhkp.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3yzasyuwk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3hbkdcvdr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nnqrzjbi.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ymatocio.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bjnxsukv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3lukjbtzm.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rxhjkriw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3bfiuxfeu.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3clgolubx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3mtcgsfsh.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mbjywlep.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vpksetxm.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3clgldnxl.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3erngpbuk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3mztbaynb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3fsgoaefn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qqyschzf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3clwtggzc.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3yppnnzef.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3kwggvyfs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ubhkixhk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3gofmnajw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3onwkptxl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3crkjgkil.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3uofyisjb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3rkimqhik.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fpsfscle.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3xmbhondr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mfnynxhi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cdivmjno.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ixdekxda.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pufvwsff.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mmecplag.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rbhivoli.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tihjuqlr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nljfkehk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3cfepbslm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ozzigvgd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3juwcqxcj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3euuhxykw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tkdhkwxp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3vribxdfp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3qstypyjm.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3biiebauz.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3xheumkql.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3hcbcvzmm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zwpxoyxn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3cbnxmufl.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jhlhxyim.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3pqsulxjl.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3hsrbitmv.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qrircpox.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tnpxvwmc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3vpnfvtln.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3befdtugo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3xjtatrjb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ecbdqivk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3dktpvelk.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jxivtjjd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3cbsyafxg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3nlyedbya.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3evrmmcsv.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3monioctj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lhfxjrhy.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3lyesjchn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3smzfywsm.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gnpfvfyb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dkqpnquo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kybaykqp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3drxqrzii.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dtvzxkgu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ewwsdauf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3atqyitnq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fdosdpbj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3exzybmgs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3tallting.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3caihrsih.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3qbniehph.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3jxcustjo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3enzvwpab.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3yyuzgnmg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kpxzezrh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3dwnvhooc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dgfwxapg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wlquakjq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ztwceftd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qhaziirp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjjtidgy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rtuglike.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3yinfnfis.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3emtawknt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ikfafpsh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3edtylkus.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3iedhwlek.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vtumfieb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3qzxytrzh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bupoglrr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3rmpmjxoz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mtvfbpnt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qaafzmnx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3lizzzvtf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdechuia.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ubrownxp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqqbyaki.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3zvnyrlgo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zqtuuvnw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3kwqupagb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3tzmsgiwv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3lpichbrb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3aosfgoib.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3cqqfgfrr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3npvqmosj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3apfytvpg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zqxnnulo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vilnuqdz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3wdcvlczn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3takhdrxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcwgfdak.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ahwemcia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uycalajd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3potujsnn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3icnopufn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hepgaxip.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ypjengrz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bwdlrlpk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tjbwlszs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ywrqqumu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pvspffgl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oxhrjmqu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3zketxxgf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3cfwhfxlu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebtupcbg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jyvutpsc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zunnirjv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xhzzvvmj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3rgcjjwtr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qwyjhblb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ehhnhtpw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3axszjwpw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3evnxcsuv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfiuynho.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xshjdqan.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbxuxcze.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ssirkgwh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3icnjvgwm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3pjlwifwv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3cdphuoza.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3iiujtpqv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3gqnvrrtc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3hrljseop.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3whqkcpan.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3amcdatrj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3btwbkydv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3aheeknjo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zztwumty.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3lyjwqhnx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yizludvc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xlvzyvhx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3usgdeclp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dnuzvhhm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzdaybit.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mludtstj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ibrgkjrl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ogggsteb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nraspvin.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3nieialkv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fajhlqsr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3dgkbmlwx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yomcoahx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3azfmnfhp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vuofbprh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zxgpcacj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3drltsbkp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ecgeicjo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3abrxgsse.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bdfldipd.html


<!-- 参考信息 -->