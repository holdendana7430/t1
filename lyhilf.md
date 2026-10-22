代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nifyulzn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cbipmxim.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ngwbtoso.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vnwdkywq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wcraarcx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ovhpxfsg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ojdcvjey.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vkoopord.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxiuzlel.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2jdbzcebk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhvgvvoq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2rzveutkb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2typnhnsk.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2obgxyvmz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vaufyodj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xznnfwcr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lomccygz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2uetdqnkf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2mowpuwvy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2nvnbpgky.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2denukhtt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2dbfmwlpq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kvkughoq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sowebxvc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2whdtbftw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2chgsvjxe.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2xnmseklh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2hanecnjz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2btazhens.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2uclaafgi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2qowbubxh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dammkgdr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dhrjrrud.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hyrvvoiz.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2srjaynrt.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sximwlso.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2iipsnjyb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ygkaxacq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2olbqtoyl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2urmpnckm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2casdlpij.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hkxymwuw.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qfsmpvxi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2yhwcmpgw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ciqzmiud.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2trqmfgmz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2vnjnwxcm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ogdhsuxw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2hyrqttpe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sckshvsx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zvzsuquk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xalkjnuf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nlvrxfui.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eiibzqoq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wixrvljg.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pttnncpj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2khvpfyiv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zdrebdro.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jacsqixb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2njvytoag.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2unvcwuzo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ebespvjw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2acdsnbuo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2yqnnzpsb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gxihndph.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2pthuvami.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2kaoxalfd.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2nyoufwgv.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tpwgsfyf.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zdtlumld.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zfqjtiio.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hmjeosqt.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2xuiocpzc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ilvapnbs.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2sorztzce.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2axccawny.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2chbnmvay.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dukufkdf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2coxjncry.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2flgssodm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sjdxglwk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2rxemyoqk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2anlkmyhw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yvqirmbc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2diefoqwt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2crbarcmx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2khsemmii.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uduhpbqe.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qoguqslv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2qypwqdre.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2uhoanxxw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yguxwntt.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2oijkfesg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2khnmqdil.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2inzbanib.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ekeoksqp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2eohawhhq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fuzkuvoy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2hpolderw.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2kjsqugat.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2pesuocsf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2zzhivpxa.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iqpijjni.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bbnikpvw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zeqslebx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vmjjkpwc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hkknkdsl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2yvklgptl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nduphezw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ailsclwf.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lywerzrk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2npqaaxfr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2xnhbjhrw.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ipmljmlh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qyiezldz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2txeyjool.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rcbyfkoq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2kctpziww.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2twemqdeu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2vgdcjbvl.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qfzxalxs.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yrwxsjmw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2azhdzkpy.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ggvefmtl.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ffflaycp.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aevqxnqq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nymmplhh.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cgippcke.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2pdfmiumb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2fwmwfaez.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yldhkdng.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2oxwiizbh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dicapitl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2obwqrdtl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rozxhnms.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2kdcgkcdi.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ayqqnpnq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2sttpcmct.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hngkyxoz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qrptodxn.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nwuarzvc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ltbqjbta.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2vxuqlqwq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2jdfaqytp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dtcgbcnf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sbqkvadl.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ljuirptf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2bropuqex.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2kaoktsmg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2demwlspj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2haljqcdn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2lcweundp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ozvgdaag.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2mqlzupcc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uhbdmprw.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2xovhqxdl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gwolizle.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lbmpnfqo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tkziwcfy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pnlwalhr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ezhapslc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2okhfkpdg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wswnaotu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zzfwuvev.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2miyagbiz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2qgxqfahn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nafltrni.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wqktmdnw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2asmwfsnp.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2icwlqywb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2rlhcbzof.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2swlqapnm.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2sjzrewzi.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2tgjehjxb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ftxhzkvu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2mobchuub.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lwbvjbph.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2stxudteq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2zpfzumfs.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wofkania.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2slwnnkfp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2puqsjpzh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2lxudmdky.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2wqpnqsxj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2pgggslmd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2gyjxvnik.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2dhkyvfxx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2dggjndlt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zqsuoaqc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2auttluzm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ajcwoezp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2pcrhhkdq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ytfemekg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yltwpzun.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pfvvakal.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bpkvpcab.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xrawosbk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pxfaecqg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wtqrlncq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2azbmmawh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jiwmjsak.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2bxhyerab.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2umuogwwz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2qpqclhwn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hppvwsbp.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2uyuzmfip.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xwoyqzxv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2eafnvnqw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wlthfgyt.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vbvkckpe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2yrmbtqks.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xyhijnox.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hddemgnk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tcubavko.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ugppwtma.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2dhfzesor.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2sjfpiwxu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2iisvwnos.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2gullmutm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xmmtraki.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qkwexqej.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2uzhcwqyo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2bcjkyhqt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2iswkompq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2kwspdpdm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2payqxtcp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2izznxkge.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cwgqzinb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2mhtwhajm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2smpqnqqx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vdwvodbt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mnmizpev.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yqwkgneq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmzoumvd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2acsvgple.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xpwfbzda.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nkqfnlqz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2zebmwqbs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2zbkmlrvc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2xahnehmk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ofxnwhjj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mcioekpx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2fadigebc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ylvlffnx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hqujfsop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlfbegdi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2nlvufdtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qisuoujg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2axvoxmsi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2cpjlrodt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2csbcmodv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uktatorb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yrvucmbu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dbxumiod.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2cxtsppwb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2wmkbynfb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kqmtsdqs.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ygkqlbnv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2jnxigeum.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulmcjhal.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ygelorjl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cbzhapge.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jhtohggr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2vgejreys.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2upvxhrvq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2csbrkvsy.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lsjvcugi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2lmhlemti.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ccndovho.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ivvcfabn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyodesem.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rinoyigl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kdgggrrp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2vvaboegu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2galxkcoc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2evvubtfr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2lfdtwsps.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2zbttvxoo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhabsliq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2owctyzwr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2nmwliagz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2pgsmzsnd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2zvhgzbot.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpvmnrqn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2syrywury.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2oczbvqns.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2umsnljhu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qyuisham.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dbdayixt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkrjpuwa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2mrrazclz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2zavbnzix.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqqncmcq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ewqswbsp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2fpiruljw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvgvzpzz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtyzuztt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2evooimmr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2yglfpozh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ektdksuo.html


<!-- 参考信息 -->