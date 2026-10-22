代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sabyypcm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wbavmyji.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lbukmmfw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2djgfuwgu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2skgukrii.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2pxaawncn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dvqyarge.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nqirncsl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kxfxyqhb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ysutvqrb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vmevlbpf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xqnkzevm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtrjgrtx.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2tsxymuzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cabvydos.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2wxhblxfg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lcmudxvj.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2fljlsubj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ezjhvxzp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ccujkfrb.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pdmkvsdr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2tettvchd.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2xymsxbce.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qvvbmtsn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ykzowlzw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2pkxskqdf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ripxvmel.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wxnxswmd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2tsxnzazx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xecovetk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ndwrqpth.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2lswuomcb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vmhvtnay.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2xoeavuda.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2uqareygc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qaaqbijd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wttdkflp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2juggilkf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rknajcyr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2noplsunb.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mqqkjglz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pzdpcded.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2oeknsbqx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2gubnxknn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2tiyeiaqi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ieiyzdun.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lhxodytl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2irnzmhqp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2dudugvup.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xkfwexoo.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2pgsqclkv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2fcobtvsc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2voouxfgz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xvjaubed.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bvixdioe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xzasprjy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yaaotbpk.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lvmzjhqx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2abzdqeyz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bemkwvsn.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rrqmauwi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vayrrhve.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2fpioqebv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mnviftmb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rnwboiij.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2iczuidtc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2cmpkhmkr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2jpfsnuxg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wpvhuqhx.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2xmqgijgz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qlilmust.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nbddnooi.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2whmrfige.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jufmjgnv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qottvlem.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2idrllxha.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2tqbtgxyl.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2gwhkrayf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2rwsxkhib.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mnspiijx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2etwbgzkc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kfakibum.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2uwvczrmi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dptlfvmm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yjrvqtsl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2klqfqien.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2okiggjxj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bjjyimkq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wsulngrj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hikbemdf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bgqmyrww.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fwipdbkg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfwcdpad.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2rpvbgkqt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2uafajxru.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hhmxcqbe.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2cgquhobn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2triqqtsm.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2flcfqzml.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dksyivkk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pipyfgdc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wqrfycmo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2diugnnkm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2gwzgksvb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2splhzdvy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2kzdtnyol.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mewcoite.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jqyfhoqe.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ucqjucmh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ujgqmgfj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mpzdefry.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2wdlzerqx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2msnhsuhr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eigtidbg.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2gtkmznht.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2yeeqrgos.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2sxpsxaty.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vnwpwvtc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2enprgoss.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2itathwjy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2cgxpsumo.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2tchpffvp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2tibkkcke.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2svqmrtlc.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pdmjifhu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fzxlizzg.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ctuozvkx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vlnorxtj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wgjnqnbd.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2psfpwuhm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wmsjibct.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tcyhluva.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2zarfexhu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2bgnujnqh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kfhgwode.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jvpegvgi.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zzkypejw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2edhocico.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lnruitbm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2otcdfeau.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qbgyyxrn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2sucnkbgz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ilglvaeh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2raecsduz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kqntiszn.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dhnfceol.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2hvmdvcip.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2pvdegenu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vpwmnkkm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fcorvtmg.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2adhrvzts.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2nfqzcbmv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2mtmoepsf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xxrbnhye.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvlcsfbu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qodpstgf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2avfcaycs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2fccnrpug.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hefhvsgw.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2hoviqqjy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mmghofqp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kzafuinm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aiuyxsum.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xvvhciuc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jvequnxb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wbyjldmd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gzsboijr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bjiqxiuo.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ihpturxo.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dhcpebxs.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2oayhrycc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qtashyso.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zvqobmyb.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2sbisvvtk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2qnaeunwd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2mbeejjne.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2rbrhapmu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2zfblpkrv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bmqqnuzk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2bzgdwhnt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ibmtzsvf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2pxhkcilt.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ngcnrffl.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ahiiqvdi.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qfssuktq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2hazldcrq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2bzwayhnj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2fpzbcnvl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2rcfmxyij.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2izgjjssv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2gtdztpdl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2fsnmankb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2pevtpebm.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2wvpcnrjg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2lfqdxsdu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ukioxyvp.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2dpcarzlj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tgweseyj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2knsqqpyy.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gwbmvdey.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qfqpylzs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jcfqyamh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rwnutotm.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2mcnqzsuz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gvlqvlhz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2qckwuqwq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2eugtlgln.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2uxlhawep.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rdgcsuuo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ifooatib.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2brkkotgv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nqhehcwi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2bnhgbhmk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wudifhtv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2avcaliwa.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2efrommrd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yvtgtqqe.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qqwotpui.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2khqjdxje.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2zybxqaij.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lkpuvput.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wvktafwu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2sucnamhq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2keigzajx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qvzdjcmj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hkmuhypr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2edozfgvn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2uozskcwz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgkfwisn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2tjmniowv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2urqenigz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tacbykns.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2toazulij.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2dsetklwt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lphlfikh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sfyxzcgs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sdkqwfrr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2awrgoszq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2wzwtxkmf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkcfukky.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nkgvzdgu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2cfoviolk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2nssjrjjz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2xtnynwkl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2viumcjgg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2fkymgpgp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2eeqdqmbk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2jwenjhma.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wiihlnyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llthbqzf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2rzrzhfdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbliiomh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2gqtjveqi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2mtmtkowa.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dphqxjph.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pjneyipt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rukvsaxe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2obkwqltt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2frapoinj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2yhywjcrq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2atfhirsr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2muscczfs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2tyyktxck.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2uaoolqcm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ppnojpne.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mostcief.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nzxstesb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2quowsjrn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ixchfbag.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ebwoumdh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2hirfhhhn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2jjkdlvfd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dduppmxr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qgwmqwgc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyzzvupk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xzcbsuib.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gklmnjit.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2srajoksb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zpfgmlsn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lhugkzfj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ammjwhrw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2smgptofx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqmrdtnl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpprnxko.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2evqkcgsd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2bcnyioii.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gvyeapvs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zswdxesi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xcyhnnij.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xmsyjcne.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2hjduyykj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2progsgho.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfmvuirl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhmzrvuc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2pihacwfu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bpvfxkiw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2lhkldshn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2hxvubygn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xjuumais.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jydwwjhb.html


<!-- 参考信息 -->