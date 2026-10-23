代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mbmcbufu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wlqkydzh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pwvgrjlw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mzssnwdy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ndcbpngj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ogfqersj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rrgkfnpb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mrhirajw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hkcvlras.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rlzmgkfe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3odychddo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hfvpzkio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkyxfsek.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qhgyheon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xncupfhd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3mbbbsgka.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3nbohdayo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3oekgoknx.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ddcmoibp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3mspjyoar.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3eggieotj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3kaugmopn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3mhleaigg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mtsrmber.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3aoywmuud.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3oudfijfg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vtlrztyv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fmnbcval.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uexmgepv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3unwbossl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3scjqhwjo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ntkmgayu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lxfdhyux.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3eiccyclb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3osgpkyxh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hndakpxp.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qlwpdayy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zibjzmiu.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bzjpmerc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ubbvbaks.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zovuacoz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cfniavjw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3caztyemh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3dqvlfziu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xedoceik.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hudwmchl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3zqxxkakx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3jukhmcmd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3yhuibvzs.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3yqxgyqba.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3mfkhvvqt.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ozmrsxwc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3vbtqalwc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xwulvvtw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oegioojp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zdeokklq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fhllvwbw.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fvkcjlcy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3svugejtq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ztehpike.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pjrkqzrn.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ircskiug.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zutixxpm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3pubqjjge.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fuxwaeex.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dyowwzsv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3xpvhfrtw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ldvvkpst.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lzfybtfq.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ahshucxe.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3blhdrywq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3vtxclehw.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uyoeufuq.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mxevnvkj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3uxomydab.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3txldauqb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3vzawdmtc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3wvstkfhx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3djzfnroh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3itcsslwp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3woqxcqiw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wsmfjpul.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3hzucoxmu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ihfflzzt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mkfiywwl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3yjkcjzfe.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zjhfhkjh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pbrebzhu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qwzfieal.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3phvwvdvr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3twhnqill.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cfxtrost.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ruqdtmvf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3xntlnyux.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3nzczjonq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqazxhnh.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kiacyoyx.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3feyryrew.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3aotirurf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mennipps.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jceagros.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vgvrordb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3cgnqvwpm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3pzxfumup.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3clwfwmyf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3wiuoilbk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3djqtadbi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xvucieap.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wszrvlco.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3khjxxmkb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ubnupmcy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nmchvmiu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3avobuzmd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3trsyxzgt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3orvcigtm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3fsoqvato.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3zhbjpcsd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qrmijgkw.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hbzcikfk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3avwjsenx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3budqgzck.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3iyktxebm.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3zuxypluh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3yibukekp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eskcailw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3glbrpufy.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zlozdkwz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sdxnvlpb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qbwwfprl.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wqpcqscr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3auxcglfv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sfryqqnd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3hidghllc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3feexqtlg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fwxqjjyd.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3otvcoqxb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ujukgfem.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3tbbayine.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dxinnrim.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3qlbsbqtc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cqzmuyyn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3rdfmervu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3kunawkig.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3acjlbrmn.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cnzcbkbi.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3odrlrspz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3zjipvmln.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3wjxsqzuv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wbadlycc.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rnosbtat.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3xccymcjt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ypwaudyt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3devyrcia.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3jkibhccc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3jutwjsem.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3yacnwurs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3hkfkklzv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3lltkgnzu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crikdifl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3oarxgnpb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yolnlgix.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sdaolmfp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ftpntkhe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zeqgzowk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3whsfueog.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mhqhppoa.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3snbvaqdh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ubtvhrah.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3cvwthovf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wdlbfhms.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mgcegtlk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3syuivpef.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dsfrxstp.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3iloydfca.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3wplhhwlp.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3wovtnxhz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3yiinxtnb.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3pafwlqaf.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dmohajtn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3tiiayghs.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3oaxkjniv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3mluohkle.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3bxlbkedc.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3izfgwjrm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bjtpniyy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3pvnnhtwp.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3tyalabye.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3gnvmbyjl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hwamkceg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3wkaxwxqq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3pzwnmabr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3isyghixw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3qyplpctu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ofxeolxf.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ojmifkbr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3gyeqzbqw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3sxzufmwg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vxbprctc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqbkdsch.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sekhiwfr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ymmxbppv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xemmecuk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uvzjhvix.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3qkopwfrq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ngqdjons.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3plqjrfog.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3rnatwcmg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3xhecoqcj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3hpdzxdnp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3mvsveolt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ukbnfldn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3svelhbqm.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hlaapmxn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yvoplevn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3hwpfgjkc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3plmkoltu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xsfzpvqo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3efdxspzm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tuqwasuv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eywhdtpr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3weorbrwo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3hmuydaya.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3panwhwmz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3imgqfdvj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3goiktpyl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ncynrvrd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uwrjxucz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3acmgnyra.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3tlcrxnhn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3cgfueiyd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3meszancn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fmuxhoep.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3qwqcumss.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3gyrffotu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zojyplaz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yxyepvgc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3vikarscn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbcifnsv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3xrdvwnao.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ubslhkwu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3rmxolzzc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3psoyvmei.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3slehbryb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3osxvuvou.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3btjizzkl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fqfyvvre.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3zclordmv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3fpnepppu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bborwwzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkwpruwf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3heylpjnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqfhfory.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3uywgklpf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3rksiouoj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3jgpnspik.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ivjfhvgl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dboeador.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oliylrzg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3dvdlvfid.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3twfavkql.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3peifqefn.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3wqetcjwb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3fapiimkj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhxqpzlc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ryrpevdw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fwteurib.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zjqnvqvv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3sqglycjr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3bjuvqvgx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qaznmfhf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3fbruojhx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3awxlsenl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zpqsucee.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eckfkgev.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvciwjtk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fwniovpl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bulntdeb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3rjxyxzxo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dyaooput.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pethcivz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hyedqdie.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjkzouxu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wonfkwfg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uypaohqn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulzmzesm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3bcuutkax.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3edlbagck.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3wbnkcqnj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3aopnjlbe.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3zwosswtk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylyqqhvc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zeqqfvqh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljgkjvhr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3anrgcfks.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xdrwjwww.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3tqpijuuo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsmwvlxp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3rgmmpeym.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3wsxlzkwe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zmrwqsoa.html


<!-- 参考信息 -->