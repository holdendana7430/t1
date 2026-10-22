代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xryierdo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nsgcssok.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dgfzbatv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2voydhgqn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lxnatnko.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2unscqcsa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pqitwcvs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uvpcnapg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jicjlxha.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2rabdwcan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wyjtpwnk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2feuyvvaa.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ieaifbsq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2jrlxbnio.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wiutkvxk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ypdrfuub.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2elisgynw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2lbraicek.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2ddiflzlg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2atpvrcuv.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2rzlvydvi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ouroydjj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uolizxgl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2atcceqcp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gqhnaxlt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gtlcsebj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2oedpylzq.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2fsflxjld.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2updypbgp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2kdkctleg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2dejwsist.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aqwfaiak.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vuibhpcv.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kkinyfhg.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yvrjvfwc.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sopwuiso.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2wockjusd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2idrpxfnj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ssrxqkyy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2hoxwtyqd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2rvwchsir.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ypzrlfay.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gvnaxkxv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2juiycqui.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ufltnsey.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2umbqgeon.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2zudayzfg.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2purmgzme.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2fdwooeoz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eodomcbm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dqcgxswx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2phptfakr.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hwudrmps.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ncdzxubs.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hffphmhc.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cxgrzohy.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zmrkbnwo.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ltrsqnqr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2zangcvvj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xgqxxmms.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2geicnyyz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vbeeiuoi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2qrsyddib.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2aambqnev.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bkouuzht.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hcrxfytq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lhtunrdy.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ucjrqxxi.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2kbjbpnne.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2kgpwaeja.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2erjcdyzq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dukicjns.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2fimkbvcb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2basobgcu.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2cnbxncns.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bmyekbep.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2dcyyuieb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tnheovhk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2wfapizmn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tzcpcgba.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2afgyoaun.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2rmfksout.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pdicfzka.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nqxxhayw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ahqhyiwd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iuugmuvn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wcxgdfbp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2biwyfzqn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fciviwnn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2zwlgcrdf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2esqspvbd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tozwfouh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2tmjeggfa.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2hrbhbavq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2jgrkcykp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dfynkjol.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jlgwewlo.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zcfrsidv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2vhbqkcvi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2oyjklwhu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ymnmequg.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2kpvgaqlk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ynqtciir.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wzachoiy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rnigyjft.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fktozspf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cromqeit.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2jszblraa.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2udfsulqp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2udjxsdph.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2dyxtvdcw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2qbdcgtcm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2hoajnqff.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2jmecfgjl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rptisugk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bhcfmmjt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2utjhtrpi.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2inlsrdmn.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2itqsrsrr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2inzuedsx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2veygfgyb.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yzidmqox.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ulfnnotg.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qrmdunjz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ypxymwsd.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yxgvcsol.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jbjvblvl.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cdinendk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2euutmbka.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2qqfmuadw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nlmjlqim.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ggyofhrx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vzzrjslg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2nakjrjid.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rdwjfwxj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2lgejawlz.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xxhjnhjp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wmbzazjf.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hqgeqftp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ryvxxfgq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qtgebgjs.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2txmqyhwd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2gahgecqi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ydbcsacd.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2potpjdzx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qdweuqok.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2tbltsuzy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2tfmqzzyc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ppmsuiye.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2pjrjzbih.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dokqcced.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygzlbwsh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2sawyhkum.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2yolhbgjd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykhibnxh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2vpgmezbf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2scdhlwfs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jemonwmq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xulalbqu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ougxovws.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yzcudzwr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2exewslpa.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2owjpxkvl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vhsmocgg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2yhosfsao.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2iwwuqdve.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2rcixwvjq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bekjmtfq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2tndgqsnl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2wmyedcdo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2kyakldse.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ecsjqedk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2mbewhjme.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2flxwvwjg.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2eaunfqti.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2skmagpwc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2sypqbguk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cbfzpwbw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2xirengmx.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jgpvexjw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qmwyhscg.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2gnzhqptm.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2zjkpjaqv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ihgcdsnz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2lfxhxgod.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2sqdpyemg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2aiunvbci.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2bkfntpuc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ehtwqdmj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2dfrwrkuq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2swfqrivu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2qgpaflxe.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2pmxrhtsq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rsgfkqbi.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vndhdgfn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uqjesqut.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2prfwkhjq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kvhdhhlm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hdpdqzmw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2yokkqrdr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iovjkdbp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xmabcwwm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2asosvyxm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ihuvbwtk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jtwblplt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2emlplype.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2wnteuicb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zokmvefb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qfnuebhr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fogclhic.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2gxnkhbed.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvcahkbt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ploguzoa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ragjckqd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wusgyinj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2irumvjfs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pnmhmxte.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2aoeywoph.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2rcttlymb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2abgqiqow.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2pshsjfit.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2evrauwjz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2iskuvbcn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ssbzjwbw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iukikerb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2cghrwhqd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kshpfpsm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ohoewyyi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ttfbepmb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2czgwncbz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lhnaoyqa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vfwfpgdl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2elpbxcdf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2dicyrttn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2bbbkcpxq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cbgpncjc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2zsbmnhfq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2zqisuxdg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2owgicmsq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2imrdiefu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2bgwducqv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lsdhgsmc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2dmkunkzt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2wcwcbnxr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ncxynbts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bluhdvpe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2vgemfder.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcpcgljl.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ynqphihq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2mwwtxahp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2eknaejel.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hnlclbvl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tapgdmdd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hgzprkwk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2yltsignt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nxhmzepn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yczpehjx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ndibjiud.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2umjhdxmj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pntppzkv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2asbumtki.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cfitowlo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2neuojhns.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2hetjuctt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ohocpeas.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pzdnheju.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2qfkrqgyv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xhnievth.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ymyvyauo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2octxarak.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bjljyllx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tnpeiqoc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wmjlxpnr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qhrungnt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gbzvqijy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zbkatgsk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vxuddria.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2gquvwfip.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzcthceh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpkmharo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2elzhcuyy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mwcupffo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2jwkmiuou.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2gljjiwxb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ykkxwxxw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wtriixnw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lhuuqblm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2meqdqoqr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ummrrxmv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgbltqhp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2yvqduwyh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ljevrvfm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2miomtlme.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2uivmcgaw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2yajzzavf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qijxqsyg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bghtqthm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2cljdigvp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwbyyuwr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2uhgsuoar.html


<!-- 参考信息 -->