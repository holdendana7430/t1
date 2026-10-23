代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jhbmpfkc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3liixqnxu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bbusswtd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nlfowagq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkpexwqo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3hvsbrfju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohgldxqt.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3axleljew.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ynbiusob.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3katkigdh.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lazfpoqt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3knhoytzd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dnblqzuy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hwxmxvsx.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3plodmrnd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cprltorf.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3bwcfucis.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3bxezziom.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3culnmpbm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ljodsboc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3jlxiasat.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3elfxooxc.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ogcqlimq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3dsvjztrn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ehltwflg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3xnrrwruv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3qbkpeyvs.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ijjdhwaz.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rkrhfnaq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3plwnabre.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mlrcuwop.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3qakzimer.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3agaomnnn.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3umtpsnpe.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3sxzezrdj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3cjsjsrme.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fnxtxcfo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xiieylhq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3utrrhhts.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3eqpcbfup.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3vopwltjo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3knqaapkw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ioiirpud.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3vwnfpewo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ywdhfqqa.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dxbtvsrl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qlemykgo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ccxbtvyy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zmngbqcd.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qulmjdkh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3irokxvpv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3phmbjkfb.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3iglwpwdt.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xnjpjswq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3wrvrveho.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3pcnbfbhm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vbklrkdc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rtjlchaq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ioakqftg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3pqojwxxl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3txrmcrhu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3ppxwacdo.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3yufsrrvx.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3fjafixsy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3psszldlq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3hofxflps.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3jqeutuie.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3zalqjpzu.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3xtbmrnrn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3kchtoruk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3odpltsxi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tsvxcpjk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3linontzj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yxxfhqms.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3fyaimouf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iqpvrvor.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zbsjezvk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3xwumkbcd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xsympkeh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eyhzzqhh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxvtfitb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrthnoqf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqlbdmjy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qdatbdvk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nxmrbsvf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3rlhxnnjl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3qhyuryvr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dueszzgx.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pjgxpnde.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ririkwri.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3mnxxamja.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3izfwffcr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lqlbpxgj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qmylwmvg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ksotogyz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3oxdcnrtm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3docknsrr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3vkyppehj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fyastbzd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3whbdmgxt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3emepkruy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ojfbslvr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xbttwrxz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3bkrbueho.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jjwldhqg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ayjtaevj.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ticbrrpr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3bmjtqnzg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3lzzzsikh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3hbclyceo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ltdaznbb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3lzwpxzku.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3cbwqfyjn.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3pyqftcln.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3glshmrrl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3lhoizjdo.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jineecic.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3frymlubi.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3irujamqn.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eguffngx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3agellpna.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gyuxkrss.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ncjqbiqh.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3adgdtodl.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3jcivvrdg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3seesiace.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3suqjvhcm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3knoncuuf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jkqgxses.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3vuzautlt.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vvdsudla.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3dqyjwbdf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kntbatqv.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3xhnwiafq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ibanrhuk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dxpomlto.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nwtjygir.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3arvftymf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3oxidgwrl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3fmnnaxue.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jgqcoksh.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fkgwzkqm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3hblbtnik.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ndqpjweq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3hjgaujrw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3mscursex.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3qtczppfx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3febrtxum.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3gdmauzhi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3yjposwqx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mxjqgjig.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3onkdxvhb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vyhnmmsl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uznknnuc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3enwythea.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3orandmlu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uapdglzn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ccunrdka.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3guxyralb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iririjoj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3pwyvpzvx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tjdgdsyj.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lrsonidk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yulujdrf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mjtbdxro.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3zhpeqcik.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3kngpappi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3tmusvpkh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3porznvnf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mzlnzuby.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wkoxksfy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3snorpuwa.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rmzsijdb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3bgofzxfg.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3omxmpetw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lyggwqsi.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kbmqjrqy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3nvqugrro.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3lhlaqflj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3awstebkd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3qeuahqom.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3pxunouzc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nfxqrrpm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3thbyqmvr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3dtygzexp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3quxlthci.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3venuhoxe.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3oedhedpl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3oqbudsvo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gzfhoalx.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3snvezcxh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpabclhn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lrxjejgz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zrrxfuux.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uzomfgou.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xubrmppd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3irezwsbn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ztepwlsh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3sjounljd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ydbrqspy.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3metqyqtz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3qqhvjunk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3bzfokirv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3alzfhzuw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ujcabpai.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gzlcbphi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wtodpssx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3gblciqmm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mbcmcyur.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yozhaotq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3frsjuyfz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nwtznwci.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3umtipifb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3mstyvlqw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3rbcvhtkd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3jqbulgjn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhhphrpt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ouprcafw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jkdopvlg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ffvaqdqp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwlherv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jtcxuclu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zcrmrmci.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qjyniylt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xqeskvdj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3awkdvxyk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wpuhubzx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bouoynra.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjlnfpqy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wdngzvsg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3amvzjiol.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rfjjzoob.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3houaqvxv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3dkeopoeg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3mifozbhv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3lbznzewx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ymhmfawm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xdrblcqu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3qhajfqpj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3tzpofvmf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dnoxdelb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyhjqjgc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ensutewm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyzimgrv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3rxfhteiq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3bgotfvnm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czqjhmtd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wbreifzd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qrbodrvf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fxvncrsn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3jrjuvrjc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wrjdtzsr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cairbhri.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3bgnilhml.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3sxzgxkho.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ustbfxfx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iaetjlty.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yorueywy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gatvqnzh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3hrhtiufy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3txnpcivz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3oeezaehy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wrrskckv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3sbigmnfs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tqsvkjoz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jkwmmpsg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qmfkubnt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rxdxsxtt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3waseppcp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3erkotmed.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dkttolyz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ndksfueo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3bpjuofqf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdvwqbfe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxtjciec.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wszkamvu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ptdrpltp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3kxpgmfya.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rgjxgayy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3julvpbwo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ujxobniz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jzgtseox.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3zkagrydf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3abvoiaxw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ouazvfvw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oyclgrya.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vncnqsad.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wjjszlev.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eudhfblv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zhbnmfdc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3yczbjkba.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3davzdfom.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhyhqzai.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bfqslqzy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dprswzcc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ziahdscy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3koiwlqrs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3wpzisybr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3yexthobv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hnmnhast.html


<!-- 参考信息 -->