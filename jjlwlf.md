代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tukbqify.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nrkthooc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qtmheoxu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2iudatruu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ptkjijqs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ihlywpos.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2idmeoofl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jtdqtvga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkbtwqna.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2xesjqaqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mestjgnv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eaviefto.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2tszgjhql.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2gfdbwbse.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lefqkkvv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2gnrhmbal.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cekqgicv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2mltnmxqn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2zzkikzou.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xffpigfa.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2rbcnojyx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2crtuymde.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ynkrfdva.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fmjcaliu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fjyizlgm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xkmmpzty.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2cnllefap.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2dgtdials.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ihitredj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2anlpauns.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2xxoqebqx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mxirkojb.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cvnsevva.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ewyattxu.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lymixcvu.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2bbqobopj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cgocufso.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vacakico.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2txaxugcx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2durrybib.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2myhetlvu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kbegsksf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2asrfgnhr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2dxketkzv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2binenvtd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2okbnncgg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2egrodvzu.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2eowahjhk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2whifcaxp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ssbwtkit.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hyftrped.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2trextbye.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2djsusuhg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tafftamc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2knjusnvr.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2haoswilp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cvcmaptv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2mrrrofot.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2blqbglem.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2eqpvoady.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hxkzakpk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ifimzbtq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ypszjlbw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2dewpsogm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2fcyzhcwk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xajcsjom.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2irfciahr.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2pkqfoggu.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kbwvncss.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2huhmldqj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ipclojja.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2dunbadfv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2bfbzqevo.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ycfrjikr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2mkgpnnrw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aiwnzxjl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2hyginlsw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jircplco.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2kinpilbq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bdxcizny.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2atmidgkq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2vzgqaxxg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2oudlddib.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2eftzxzit.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vwwtkzqg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tbbgeawv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwqcducq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tkgccwjh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fndbryzw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2smfjpkcp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2guxtngpv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmzyhrno.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2sqgrawnl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ixzvhwqo.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ahxdxiqy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rceastbr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tbsczakj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2avbuixgr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ctmhtjwd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2nrecflhc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2bowvxjdy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2dxlceznz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cczukbwu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ytpxpcsd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2afgvjgcy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fqrhgbwo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ktnulxvx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2vxohbqzi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ucxljayy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2afxvfobu.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ewyerpjb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2jzkhjvcg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2buniunxx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ntmhvdhl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2yltddqss.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rnrneles.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2phsjkiil.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2gliryruz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2xdbtojmv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2xgnghgqd.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lubykbqd.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2udiifdmp.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eckptnaz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2voacuzik.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qaepuigk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lxndlefe.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2idojukby.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rwswbtjj.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2uyanehhe.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2xmrwiivg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2adknzfkq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ymwdrqay.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mqnlkbcp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2otfxxzfr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oimgxtyv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2avncxkoo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dhlljfae.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xeinagcr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jcezcass.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hrxhspxe.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mxubtatv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vdgrpdam.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2evrvmvlg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ghsxqucz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2eechmzcl.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2etjniqtc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ktxsgrtb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zjcnezvc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2prxocslz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jsenowzt.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2hidmfngz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2vtlhgaau.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2wfvjexfk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2dwibkbfe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2erlsjppy.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2dvswbmsw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rqzmtewb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cbnlbesf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uvnetblr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vodhkyxs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2osuxvrqx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ortijzia.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2srjfwsiz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zoszfhmi.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2cyviftuw.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2faoehsby.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jrtpfihc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2evzmlcww.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2meawoshy.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2nqohncki.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2sukgyupx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2imjtudxm.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2hgbqwfsl.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2gbuyfdra.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2formgqpx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2zewwnbso.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ggeopmor.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2smpaxrvx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2xuquihsq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vqjnhyto.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dzquefoj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2mqivsuvq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jrrexmuh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ahsdxzui.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2byrakzcx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ebzkjjao.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2nslrrzyb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2yqqujyte.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2rrtcxdzt.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2pengchbo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2peefmjhl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2iseyhfdx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2jtdfzsgq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xtkuduzx.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwggcxqy.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlijvmpq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dqmoczqr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vndzruji.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2swtimlma.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2eqhowbth.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kauhyqnr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2tmgosupd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2oxrzflrr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2mznisogx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bpasftyx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2rtnsfopw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aigposts.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kclqddry.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2npojkevg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nqmhoawh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2xstimcyt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2meaedtnd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uiemwiyb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uvaqyykf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2brlcfsfm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jrrrmlon.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vxofktux.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2uxnsvnky.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2axpczekd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2yzjxivzn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lipvqwjg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ntqyvxyq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qpvjelzh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2owcspcnc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zmabqkkf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2earmbarm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2sgnzswvc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2samofjkh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2rwkupnqi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sadnzwne.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2udfozrcc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rtpewjmg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pxshbzes.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsqjwqhu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2akcaxlhu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uqhfmgyr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2lwfqxytx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2pychpjmz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ujuzcmma.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2yuoxcjzb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2hruoktqk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gnwsxmxo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jpgqsxrk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sqcjxjzk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2apciysvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kimtzwqx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2anpqbupw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zthysshm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2njyqhwui.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2arhmppma.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obxjackq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mmjzqnsa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ozgqexhv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zvftqfgp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2njkzkswk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2tklcsamc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mdrsvhyj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vpeielpy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2aiwyvdpf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgzkwvet.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vlfgnubi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ftiaudwf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ljaogvew.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2osnbvqcy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2pcvqyspi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nxwxfckz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ukupsmwq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2uugakufs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqqwksxu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eounksqm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jorrvxmg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hstcgmkb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2iwjyfxse.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2jbgfeinf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2datcxpfo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tqaqmoob.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ekymbduc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqnrfimk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqewhjcx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mrfqduyz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxuyhwuw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2cucyyvcl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ewfpwcjy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2xyvymguy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ydjjadcv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2semwmmxv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ylozawxs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtpcpzun.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2aikgvmdd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2vmrkugre.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2cozvlljq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2duuyeati.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2iwdakcup.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2zlztsbsp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hyvlvuod.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mcejergw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqmkwjox.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xbwfsdkq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysxlpmnh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rttsyyru.html


<!-- 参考信息 -->