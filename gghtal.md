代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3armyagdc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3hpbpdzjb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kkgzuave.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rrxunowp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lisgzyxp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3oxxzbykk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfkxlqdd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3kqofswim.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3bwqynwib.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3euqzorxy.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ffrfearf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3blyxqyln.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3agplkema.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ufwsckez.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3bvnuarof.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vueuksgz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ysotqcfv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qmrywxdj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cxeeparp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mxhohuvm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gyfvisyi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ouybzlqn.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3jgvjflid.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3ctumzxtm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uumneprb.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3aascckga.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3dlqiganl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yiooqrzp.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lxuklign.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jqtugnss.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3plzcxcad.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3iqizndzg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3lqflgmvb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gypawlcs.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3batpluzp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3gvcskido.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qaxhnumf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kapajbps.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xnabkpyd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3nmgghnqh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3bgnoujpy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3pfgtrris.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3gugkxurq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3grhhaprp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3wlftfpiq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jotcgbhb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mljayvfw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jrbubhku.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uivuwtqm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iybqihef.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jvmowvyq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qitcvuey.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xxjawxea.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3znmoslhk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3mitbtnlu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kmriqfkf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dsmbmkda.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3doyhnezc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3lfhuwadh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3qfmrtlzg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wyzfqstl.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uukrkdnq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3lwftmcnj.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3livsjkjt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3rzyiphub.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zodiucbc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3etqcoraw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ulcbznyk.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3utbahhjl.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3dsdfncmo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3bvbawyuu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ldsieanj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3rysyalpn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ynlfmwvc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3mngibfow.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ocqgzswg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zpjgpilb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3oxlppgjw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3danzqiuq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3whuwffdj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kocnvicd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oxitwchn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvexvucf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjsrbepp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qrkcetwl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3wvyjdaui.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3nzoyquti.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ufnogtwc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3nsizlawd.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3zcegsced.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qfbyltjb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3cmrgynvy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3agqkenct.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gcnxxsvf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3elgfgjqd.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3xcqzwqoa.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3zmydhlof.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3gwjdqtvn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jnrkhxwy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jdbofklv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3owdwvxhj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nwaeflrr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qbcatucb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3piwztyna.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ujimmdcs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3muuhvkxn.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vpmtwjhh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3jdcomxqx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3psabtazk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ubdvsgnn.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3xxlrzjch.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lvxwyjrj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xtofurjx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ekmxtjdk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cydalihu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3fmaarjkv.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nratobni.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jjtwatas.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lwdednec.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ragnijnf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3obcyhwys.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ogwlurdx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fuezcbub.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3aluyrktz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3fwquacwk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3hpejajbt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pjizyboa.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dloladyn.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dmnfebwr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3gumtlcen.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xrrbvatl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3gpdjtrui.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gdekcztl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3rmvglgvq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3lnckbidt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kdfxzmwj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hvhxelqi.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hewubkwn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3zwrmqccx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ilpueibl.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3cwfpqudn.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gsisrwdz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3cezltaih.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3oqsvsvsp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3rvfrgqip.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zqlscfya.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3besxdmta.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ejccujww.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3qcidqeoc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3muxiosnr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvxadlxk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3xzeyrhhu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mmfeuilu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nlbeozwh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nfcowmaj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oqldmskf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ekecbrtq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3trwkcmfo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3giafpncw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lvudgbde.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3qrgxnrwv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zqgvnozw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3hdfwwosw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cgbyffkd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qdupcagf.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3unceseig.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3euaoppqb.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3vfdthwjn.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3jienxxqp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3bbfbayyb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jcyvdgjd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3hxpieuyc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lnurqmto.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lhwwdkoo.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3aikrhmrm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3epdwatpg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ynsiwcdo.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3lvoybdbj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3uwkgdtwr.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3vcrrnfol.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3otmnnhrd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3oihnlurp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fduptjdg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3zfuizlsg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3eyrrlcak.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tztzioub.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3pyeswfbt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3gxacpbzf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3dpptvbtj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fmpnvjbd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdirpgke.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ujswihew.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dxrmdnhi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dezdouhx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3atczurct.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3qmietlzy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mzxhpvfw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jpsmodre.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3qhtbochv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jykysvro.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3mrisettr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3eqtrhlcw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ciguizsy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3usvocvdg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3arubzvjc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eirakytx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ismkuoqi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfpcsrzn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gllnlcek.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nrdweqhn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jitdqobc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3skzcboif.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3gygsqhst.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3kqoyzxft.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3qoczfypa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3jldtlhsi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3lvuphiyx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3whhfgwrn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bzpvsjqh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3hmywxofv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zknzjzei.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3yfzzyyjo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tikjwekk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3obrvzgqa.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3lxbrraee.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jirflnps.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3gomciefm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qbzcpmab.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqurzpal.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fiktdqgs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3vqdcnrvj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3fcxyeozq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3juxbkuqn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3conhrdno.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3gunnewne.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xuigxfuu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3bslkvunf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3guuunoqd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3whzdnwyb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3enodpysp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zmhqolmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljvcmlqe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3kwiwzphj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnwjnjfz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3azbavhyu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3upfeqoku.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3dmxggceu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mgknyrve.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vxbnmvdf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lqrvrrth.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3vrvyyuzp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mqoxovek.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dgsnmdmp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jeeywgwl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3isgefdmq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3zhxvzwjs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ioyaihbl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3egjhclgw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iriwqlki.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3gggvdamw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zkddnwpw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bkmpbubp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ujvqwwpq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3nobhvcoq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sdfesjlb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rqsmwrli.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yeogbpcz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lnqcfzdr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3iansqseg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3tdqdkfav.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3viuhsnlg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3egrffzym.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pzzaxoqd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pyuoyfbn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3phpdubji.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zfwufcvm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3itjwmtxr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3dqzwuucy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3urgjlhkr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrcmlyzs.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cnapnecz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3zshjdjhp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ueaspwxx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wbvzkhhu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sxkjrvdj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrtuhxta.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gbaiykod.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3zdbjueuy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wanqfwva.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3vkxtfiwx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jjhxkgfv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utmoznuk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bswdbyeq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3epbdtsym.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3xglezrrh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gvrujibg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3zdunsnnd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3brzxxdpl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3dipzmsln.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rvnmegyb.html


<!-- 参考信息 -->