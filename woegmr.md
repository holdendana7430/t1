代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cnixdnyu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3qcqymmzo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3oipxpewg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3itmomyil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxrqqlav.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3gkojjqjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skdjjbgf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kkbohxhx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3fnpzcvye.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3amqqdpuy.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vsqfvkcj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3pnnhunit.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ndymabvo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3wwwitzyj.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3wjavdvcb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kartzhue.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3hnblhkig.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3dsxvtvqq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wxqskftx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3awbmkral.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3mkeiygdh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jyjbcvqo.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3oqxowvwd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3jdskknyk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jkjgyzfs.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3octextld.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3gfodryxt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bxcvpadh.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ypcgbzqw.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pfsxexlu.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rmixgvhf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3sydvjfdu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3kznplsfo.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yvlsxksv.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dfckwfdr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3vpfckjni.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ndawkaai.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ovoupbzs.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3allvbrtq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3qkfnblyl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3zsxqrcyp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3bqfpukbg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3tbbcjiui.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3hcqcsdlj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3unfgfnip.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gpyybkxk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3amuptipi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ueeddiqf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ecjandqd.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xtyvduus.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rimmsnks.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ylqmoccn.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3trgstwoz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3eoegsugw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3wnxxkzyi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3sxbynhxu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qdlknuzd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bgssddax.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3rececymj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3mzhbvkeu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pfofgukp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hopkticu.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3olobdrro.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3olnwxzmz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3flpmdygv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3pldklkyj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3zcdjgnpg.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ocpdunzx.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3emrypbeb.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qdfbxltv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3zndlxjnf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jnmvovax.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3jthqqmrs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mhprwzgb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3rxkhpfpb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vsrintfx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nrmceqrm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3bzrputvv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fbtfydzv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3azxfqddk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bjychcfp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3siwjnkkv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzuypmer.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3unerudnw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vailaqgu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3wpbceydm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3vjxxqvcp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xvknzgdr.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nwzytkdy.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3rjswtuyz.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ygmrnveh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3innieuht.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uaklrhzh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cerrtpwp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3paieefhw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3kqegipir.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3uciwdqba.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3pfmxamgu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3tivmldai.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3swlqdhgg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kgdkbruh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3guyedbkq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3whvhzplm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wxixppwk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tpsfzeil.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vzckzzmt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jdbdcxmz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3spxtepbm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3fclzhecx.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3umbmzhlq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jffxahfd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3mmofarwh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ihuaidrz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3wtaownyo.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ntcchlnw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3lnmrrrvn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3patzxluq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3djdjtlul.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uefwppfi.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lybukbxk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jotlnijo.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dvgupzbi.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zppuziit.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hevlrgcb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3kprbtxtd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3svyhijwx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gdttujya.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bfohvnuv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tsnwdfiq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3qfuqmefx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ektpimpm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3xqtksadq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3auhgryrn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3yefxqswe.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qrbqztyg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3scqwxcyr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ljqsvbti.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qpflhxct.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3apejewju.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3yycwjtrf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3sxlmmduq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3szinaxqv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3hvalvfqo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3jqzhuhfi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3avjpifda.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3sanklars.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3qnkrgeil.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3hydksyid.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3spzgbrrx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3otvktpgp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqrsjbxb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3lphyybwt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wzlwotev.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qnapvous.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xzvzxpik.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ewhfekfy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3agnyixee.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wulaxkeu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qaxlltdl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dqrjzkoc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3outwwjgo.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3cdtikzem.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zfppijoe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qanhwydi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3irtbxerd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3blasffzn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3abudkknw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3iscrcuue.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ixmogaoh.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3riofepui.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dtaauegk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3yaqnmbhu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ygbthsaz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3enobggiv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3wraaatxa.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yvfwktdt.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ggejmaal.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3gdulanha.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3azijzuhi.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ewetbbrr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3yaymhnmz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3hepzouyg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vjjwjeva.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3zkvqpara.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3yjkdzexe.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ixhhfqfm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3lidjnnnm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3vcbnfugj.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3anejiyih.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mvfikbpb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ccaumgrs.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebcwgmqq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lbraktae.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rxdjkgby.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iuemkdzd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3pqzyxwpu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3phewucja.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mfotpxpx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3kowyoywt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3vqhmyutz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3posfepya.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3qvjqryld.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3fiqptjww.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pzbrwxpt.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3syrtfdfb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nzlnfwnx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uzbjlxup.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3gndfbmjm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3chfaqmhh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xmpekrxt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3aopoiemh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iioazuwr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bksodlgw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3fnhyvvnh.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ptkpojxu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3tpucesjc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ltwlfnze.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3drddxenr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lbwukyqq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3bgyxqkee.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3flfbugpl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lapyjejv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ecsqvbiz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jcosmmdh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3imlwlxgt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwykudgz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tlirhpzu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lfhqizli.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kcczqhby.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yenwsiir.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3hhrlevxz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vckgcpnc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3eagmnwmx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3thqqehpf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rbmvumik.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3evjywqxf.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3tvjhjxdm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3kdsnvtlc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3nrfdiooe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ugvdofde.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tonamiex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfwxxima.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3woalnlaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eaedupda.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ispfljej.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fufyytzp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3eqdscfts.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3auuqxkmb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nbtfduad.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3aarxijqc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3nnhpcxss.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3sfvnpwsw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rlbrhbxp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3kzevbabt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3oqsxqaic.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmxxsesd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uxsfquul.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zwogmefu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3becxzedz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3iueshrle.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3dwrrxnla.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bbciajjs.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qjwxoeur.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3wbuwxodg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jkwbcorc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdichubk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iubichcf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qihugviy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qykfdjal.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3knksibhw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cyrvhivf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3oxnbvtjr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3vuaqqrhp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqnpntsu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wkjmdjrc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3noezxelx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bppuracu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3cuobuzzb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kcmnqpyb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujrnbhwj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yqiupxzu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3hqcwixsu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qcvdllon.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3uembgsnt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3prqjtbeo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3swehvmhn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3smlwwfea.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3iekrudtz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvhuqpnt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ygmcokeg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3possfkla.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejhdvcqi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwmzkoao.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlexhjdx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mogyoxnf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3bwbkatbd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bnsfwqju.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbzcpuvr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3oomeskeo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3xmckgkbi.html


<!-- 参考信息 -->