代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3keyjkjwl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3faxuqxie.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zdocpnah.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qkcqdqkx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vmzjpqpy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hyvdinba.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xvponhcx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hkfdnumv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqbpeodw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3zhjowxji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmtnprcj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ouytgumi.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3wufplbhn.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3daugxeyt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fpsbzune.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3znzdntxc.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tjdoiuhx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3mknejeyt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3alfdsmpt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xmdkrniz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ortcjqxa.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ktfsgztn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3konvsccc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qqweifku.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3lavqzjof.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3skxsxuwn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3xisebggu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3tmlkelaz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wdkqfhmv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3mwhlvjdl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3rlungmot.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3whzudhsi.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uzrjvfoy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rzxebdyp.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3swslnnzy.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3qihduxyd.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3qywsgzbk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3plytvhpl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3payxdood.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3hdrcdhco.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3wlynamdr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3auujqwfv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gtqcxvmb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3rwtfucyv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3tliqmhjd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3jxicggns.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3pnzihpfx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ibtpazjz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ekvtyhzj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ypiqslsl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fyslmzpa.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rwofnsze.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bqyxpovj.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qdkdwzds.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cedmdkxr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rfjwiaou.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3iunwkrrw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jdebcjam.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kuccxnrb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3jmqbhujs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kavvaxbf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jzkvmrew.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3gjjtzaoh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3oatiamoq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3veiotfku.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3xxfdcnhr.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ustxjubl.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3urucvpvm.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3bjkkvijn.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3tyabtngx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rmkbequv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hoobbsjb.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3mycqvdtj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ahzywere.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3iiczbnjm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ddxhfqbs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewlgpgna.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ffsavrld.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3xqpmwvis.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3iujxqkzf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fdqwrimu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3hsblovfj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hizzulef.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jrijthhz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mwshdxel.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hektlmgn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3smmorbsd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lcekqlur.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iubotkhi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3tyxfeblu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3tutxpksu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zmlljuaa.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3sinqjfjc.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3nsvhjynm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3gwolhetq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3klcytomx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xstsotsf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ctreqoze.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3byecrdio.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3bbdmevap.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3xvxiokkd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3oplknvqz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uaymajfl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nyfprlmd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qvdjrroh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3itorjctm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uvjdybeu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3qjnuguwu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uopviaqa.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qbucmyhp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3aitalmbr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3allwmktt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3qyfldodg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3yapqtydn.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3sxximbap.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3jpywvupt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ehhhkenm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3gcgcidfl.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3nqksdxrs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3gxnwqdxx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gpxtzooe.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dwuhiiym.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bhhgsmgv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3snqfqhcq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wlbxawkk.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3trvrkiwf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fobzgfnt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uljkpkin.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3sodjzutg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3iyviqflq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lkvkffeu.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nlrgigza.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hpiroxoi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3phwuvrrq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vrnzcxde.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3femigwqn.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yaokeysb.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3nmbjhhmi.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3khqgvafm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jssxvlhy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rfkxvzlw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rvqveere.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ociuaaio.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3jykauqla.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rydbhkrv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3iwmpgqbp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3easgesqv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kvdiudrs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3zfhrzduy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xhgfqhbs.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjmzkgai.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddfsyqpy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3qmmrbnxj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3biqnzpnm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wwlnyzev.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3jbkeiafu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3belhkzrw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kdxcklum.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iadapmdn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3duxnhsmt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gdqlebya.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xjjyvvrp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3naavdvtf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fqsrgnvt.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3elrpbklq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3piatcmgx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3rvmrtmlm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xucomjov.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tbzmulef.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3woqnflcy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3cdmokiex.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3olwqfrhi.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3cflprjzy.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mkhvmveq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3amsegnsi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3rjgyitbs.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xeqtlbnw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wlaafeoi.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3lkutkqfr.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hpexcthz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jzxmoufk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3lmgruhll.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wjvjbugc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3zrzrnbbr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3nqbtebuu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3gxyezspy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3akscgoga.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3tloguiea.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3tyyclmng.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3lyfquhxh.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3lwmiovow.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3pgcyzckx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3bzbmsqku.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dmtogxau.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sfbyflzz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dacmntwm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fshhvhry.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mmmkjkdn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jczpszha.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ghseckfu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ddnvykpj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmxixdnf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3mjtkjnyo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3maspawtp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jsbvlnju.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3olflbtyg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfnzpuso.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3estpcvdi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3lbrrfppp.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lpwnuezw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3cnsxwjbb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3oftqvpea.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qazmiohg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yvhkzudz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qljreynn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndwrexrg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qazuaehh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3dgqtotfr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3bussiqvx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3rtsqhasl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3cemnkrej.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nrxzdzgl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rryvghyp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3cflkufkb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3gubtdmqv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3dzuqttns.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dzdcwttw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tfqgqyue.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3esnqwwhl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3oknluiop.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dfiijsmz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3twhdzxzj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3bktbabqj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vspdqydp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3hzwkwfoz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iiqfrmpy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3vldvmwhp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3fkdrjalt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3fzkfpcfr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3bmjuhkzd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3sgexuwyc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lahzhyxj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3txiviwae.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3mzpwcnmw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xbjkzdhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kylefzmv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3uhmoktbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvgmcbxg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xtgeddvb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ukcubaaq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3gkkwejpa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kilhfqbk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nplqhdxs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qpikopze.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3xtrizhnd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3nwcaunkm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3iwczbqtj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3kzhshgib.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3bgmocufv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3hvdbmpbh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kcvmyhyl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yycjjewh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lkwzypgv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3coyuuxuu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3hpyrozeb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hhjtggbg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3bzqudbmb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3jzndobli.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuwfdcyn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pofswkbp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3unvcuwwh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfxxpspk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ttovloqs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3wikezsdu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3crljjdrt.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3uzjktvof.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3czzybzyd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvcnjdsp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjppvzqo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wyxunqby.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfaxsvkw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ydjhtjsz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ctaqryee.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrciewvc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3djidkbwm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3khuphedr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3luerivgf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bskubcsi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ndvlhkoc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3loyjvlzm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vcnpmnjy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3idllnmpp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdgrxgcy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kexvjmeu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rsluzcqe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvdwqcmf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dfatlpgc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3xxtbvkru.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wujhgnvv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ubzkjrxu.html


<!-- 参考信息 -->