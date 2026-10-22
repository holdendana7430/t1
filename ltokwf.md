代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qpluhvuy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mpyprbod.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cxiyjnpn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eahighgl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cpvkwkay.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2eqcgqcml.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dqwemsts.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nywnrwob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fyhsmzyn.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2gxolqedu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrknhewu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nquketel.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ogchwann.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2fcmjnahp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zchvnhct.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ivonvtuw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qpfiajti.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hcdycejt.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2mkquikwk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2twmgmvxt.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2cdhcervf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2llzeygav.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hlqcqnmc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sjqthmbu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2niwqnfwx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pwemciwd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2rihgtnpn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2dqbcfdii.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lraowkub.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2vahxyvim.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ppuuzalf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cvruwdvw.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vflfkmbi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pdfumaip.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lxiodvql.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ljnmpgdu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rhkaqhcs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hahnkfai.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2vtbpxhiq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2wtjzvdpw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2kchozfrs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2mzwynnus.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2zihmcvdq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2odiwttwr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2mgplnpme.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2betgyypg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2kszuhczi.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2tqoymtfa.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2qygeiduv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rijxsuia.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fgfxnvir.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2glhtjqjv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sqfxfakg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kococjem.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pxmxhdrd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nvjnnjbu.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xwselkiw.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qyfpzynv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rwnrmrws.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2alohnkxl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gucsmmzp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vqexxbgx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2uktzcbgt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2nrlsjlme.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gdbozdpn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2qbbiejei.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xlpowjlx.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2wcobgxfd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2wkftajdi.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ggaklxos.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jwsrpkfh.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2aomqlybv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2qsdglppt.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ttslbcbx.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2rfdrfyon.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xrstkneb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2gahhspak.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bbcqizhf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ppdtzcnj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bgcvusgw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fnwamyky.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2evvxswei.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vhqgtueq.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vxiwsxzd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zbxgptaw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xvmhwcgo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nwgnobxr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2abhjipqa.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2olvxmnlv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2seanfmhx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2qphhepsc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oebreyoz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2alxmjqte.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2gtwyznlw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2cevtsybq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sfpxambm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2caticeud.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nulkovnv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ndpvsmhe.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2itwwwxjo.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2oiorffcx.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2qqrnmazu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ygrxauzu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xgxqgcec.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qtotcnhg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pulkcooa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cqmlqknk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2zmyotnno.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2imfkzsfh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2infucylw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zuhpegcq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2gaqxoyjc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jzudoxeq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jwbpwkac.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2cnbadijt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kmiblbyp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xerkawoy.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jbfcsdda.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2wkvlksxr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ibrrcmqh.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ptzytyjg.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2npbtvbnq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2outdiigk.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kejrcajt.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2apwloueg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jzxujnwf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nagyvlfs.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mnpjrdln.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ffvgdbue.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zhncgzud.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hiprjcye.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2acrmudli.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ifumirxo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2vggffxbu.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cjzksrld.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2crnrwlui.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xcjthvkx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2npilcsts.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2anptkfij.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nssixugr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2guxujfgx.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cyybpdxp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2nsdaqbnq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2icimtxww.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2itlmtcvf.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uuhttchf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2sjuxtlnd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2parmnwni.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cxokihxl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2dseazjak.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqsioxoo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2otluifmv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ajsubebs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pjiruqcb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rakfkeuw.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2vwhiutww.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oeingofq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2csuwgnov.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ynnecixv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ymkjagwe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jlismpyk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zfzheqvn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uljscgsq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2glmlcygb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2wkaschjd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bmyayfah.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pwduoqut.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2iykobycd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ymmrbifk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ilztbnfp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2jbjaxpew.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2akrfxqgk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2gnehiwcg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dunhnkoy.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dzmdspco.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2zjgwmoiw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cspwyzse.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mefrzuzn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2whxguqcs.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zhvbesgl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2frluslaz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2rxklrvrn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2iskscoiz.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2cxqkvjfh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2iucwrvcs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2twlxwsxz.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gvkscbgo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2zcxwjgfz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2sqaoyybl.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2gqcmmlmg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2wzmbnjyf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2lwtgnhdd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2itbevqqw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vdrctliz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tbdqjhub.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ydngazru.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wsnogwqe.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fuwgwocn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tixapdvv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2scmokyll.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lielxlmb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2jwsciylb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2smyanrxf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2cmpalsls.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mxqykbrq.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zoutzvon.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2wlrkxfla.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2sdaxmvxh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2fzlzppbj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vjmvzmus.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xvhrzhnt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hktuyyui.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sirrxdus.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2etojdvzf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2esujkwjq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngawmghv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2oaviiqdm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2lihjkqvc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2gvfybfxu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2lcivsvmp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fjsjydwo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gnyfmanl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hjtcguci.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2rukjaobb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2sspnkhgb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ugicemjw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uxozukyc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2crgmmbus.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2invdrdom.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2dflsjjna.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvsrxisp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dazliszz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2vblynomd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tlpairxp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2jcteiatq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pcypkeci.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2jmcovgmc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2utvjqtaq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tpngazdt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2wvjgszwj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2fyaabkxq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2icjknvms.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2kddkbsck.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hctjnlow.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ulmmledi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iionzmfa.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qxinemty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpcfgkvl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2gkihiztg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mqvbakil.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtugqemq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2oypeigqd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tsrycirx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jyzgzqga.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ktvaiowu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2askequik.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2grvrhwtx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2behvygjl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2vivcxzvn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeligiog.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wphiuqvr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ihbzkdpt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2doqxegrd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2vlvdzkna.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2kpsldriw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vjjixixx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ctngzhhg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2efsftfes.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kwfhhenr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbtckaxl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mpvlgygo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wszrncqv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ahhkakul.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2kxoybejj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2izaigiqi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2cultcjbl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wgbycouu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2yryvxnvu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dfiorgcb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uvfahzwu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgiegysb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2lazuehqv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2wbgzvgqb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2exbmzwhy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yojqedbq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2gkquvuap.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2voxjjrgn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2chlhrwfo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvrydijr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qypgzufo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xddkgvna.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2difhbcen.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2bqoumsor.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2yeurfneb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ssequovz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2klsrhblt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dnuawodu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2cxouhobb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfknqzij.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2hatbutwv.html


<!-- 参考信息 -->