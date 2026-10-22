代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2jsfvupqy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jyynnghu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dytduxzu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dfxwhwzj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ecdxxala.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ottvoiop.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xcvxuwzm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2sobidhtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aljxkdkf.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2zxsxdvma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akvwfblo.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cygcipwa.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wxuqpcxy.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2reqekrpf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2acrmupvz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ysikvoap.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tzmlyfaf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2eetfdeib.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2xqxbusvz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kcaycrye.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2lwysyrml.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2cnazpugi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kwrfihdx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ngotcehw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2eywzukgl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ackdfhxc.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2gnsuyxrz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2pcslhkns.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yxfwoylk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2bmsumuuv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2flayhicd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2toifynqt.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2biwtesfn.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jagzyqns.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2knejqcrx.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2blassbyx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jpuvajnf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dgbwnyxg.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2iikxrvzx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2isdihyhv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lytoegwr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lewqeocm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2nhgiyzsl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2gqpdahfb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2eyaecadp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2xtsqyfcq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2jqcscchu.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2qyfeukxs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2xoibhfau.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zcuangew.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rejspoit.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2whrwytzu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ftqgdlkg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2udrqcrbc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dtewdvvo.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uggjzica.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kcblchdo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2knukvitv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2kxytzoiz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cirbruam.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rpfkiabp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wpplfula.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2oopthtfg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2emtajyek.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2snxuvmwu.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qidlkneg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2nsslzstw.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2viwsfnnh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2vmkviuym.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cswguckc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2gleijvmg.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2sfatcrju.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2cictmizj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kmiullfn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2kajtpfap.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tdugypoh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2yaoyqrvk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tmppgnkh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2vkvtpwkq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qohgjzky.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lcpzoddt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2uttjdymu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2oavemott.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cjjzhvlo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2azssjgdu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vhmhkewp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dthgzqno.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hsahfxlr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ccsbjieb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2alricxqh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2kthynfkn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fbrmohta.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lpwjygtd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2mfxeozlu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2mgiiofsv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2aeedwoyb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mnjukssi.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lcxjimue.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2pbopwqmp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2czfzxkkc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2vjyvoizo.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ykihmjtg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lanilbab.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xtbkwnrr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ntxhunwn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ofzyavyq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mbrbuvdg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2pjkfmxlu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nrmbjafz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ybhfrnrp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2glsbdqjf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ajfkuesr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2teankruv.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hpnqpaoh.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2eweqgyzp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kpfechuy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2woxqazto.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pgzeteoz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2gvozxvjp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ewopvvob.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2molvtrwc.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2svwczzdu.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nyawsbsl.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lriycoga.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2brtahnqn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ptmsgnvt.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qryusflf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zugkelay.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2hqiycsgd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2sckwzeev.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wneazsqt.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jkcyhwaw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rvloxinh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2vydxpdub.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2emefnsvd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2winklvvk.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fpjtdonq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2esmreizf.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2bkeyrtyp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cqdmlvis.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2obgvciiq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xdtopkch.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2peeghiiw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2dnbbgwlv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2sypufmhp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ygvjzovt.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xlfhrktx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2aseinvzi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2mxzndzsp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2vpyixvlh.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2kromzbrk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njkzqdxa.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2pyfllame.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xhsmfiag.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlqikrov.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2kmxmjegm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zddmvczb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cmewvgyn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jwgktzst.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2miekfkvn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ysqshfxy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rqqkgmqn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2madzqlah.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2igrzpdvf.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2wuuzxmyq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dizhfmyi.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pexklxot.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2cpojgslu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lxyfoqom.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2bvkglmko.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2bgcvvdcv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2skskvvsk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2tgjwvfxu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2rsakgmwj.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bbvlordx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2akwukhfe.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2iyfprqlw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2wernfyjb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ebvwelnm.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dlugfmti.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ckunfjoa.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2olksvwib.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ozexhrqr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2kgbkzmck.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2xznhwztp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2lsbwwsgv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2gkfwcbvn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2mjdjirxk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2towcedqy.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2hjspcvxe.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ucimmyhy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2xeqnstdt.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2wropermv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2akniwkwq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hupquvxb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ojgzufnn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fsoicyxl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wavkzppo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ojngzblv.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2mskgxmzf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rhcbczth.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yafxegon.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2xjqilsoc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2vqqczedr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2xrjmafbv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fsfvjzuw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2iwfpbfho.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2yyizliof.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pxsnvvkg.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2puwawnzd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tethisrl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2tjysjfil.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yvfnhtrv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ynglpmyx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bwjjptgd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2lmqkqowr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ordtxkmp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2gmahucaz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2gkexxqms.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2qsjskcks.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hctkildq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bsvqjbng.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gepryxyw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kgxfgkvc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2iiygmuqg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2fzgrptln.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dxmkzpff.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tmgnthgt.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2abbkqkzm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2nujpcznw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2eywohjdz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vnypbhgt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fmswshzq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dmhyteal.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2mzkholbc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2iqmtvgzi.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ywajpmzg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2khrtzrgb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ggkewiju.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2hvpnqyym.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2vnknfops.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ewwvxfbe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2zhhkryom.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2myrympsa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mposnaki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orknvxqr.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2dxqrcyzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtipqrce.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2joortopb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2sfgfwiga.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2thozksvb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wqayztkb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cdnzvatb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hynhniwl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2pogvzkqx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2smwirkps.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cytkypki.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2voqxjiwq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2gxkycnje.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcllnhjv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lxrhjubp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gxitsasn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pxvlaxoi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2blryxrtz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xdmoawom.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ltsnsdrl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ickwwuxr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vounwkho.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbtmlnkh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2juuyrhqf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zlwjtfwg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wmmhbzrj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2euibdlbk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hsjysdzp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2owyelowl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gzdviydm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2iqdhimrh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2hembekfu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kiwflqqv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hfaahgrv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2masqndes.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2giyntzzn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2dcbeugrk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2opevotdr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2mamtrzzr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xufnhaig.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2trudrxva.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tkhaysum.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmpeupsi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2dbbuwpnf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xklnhent.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xjozvtar.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2okbnlxxh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2yabqffqa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hlcvutcf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2dzchfbiu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgklollb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lohvtwvf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2shdadafp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2idgbzxui.html


<!-- 参考信息 -->