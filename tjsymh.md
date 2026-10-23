代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3khxpffpm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3thhbbyey.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jfbcopop.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jlwlcnfp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ofylwszc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pjblzwzx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jksekigz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3nurqdlcy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wsfvtyho.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nvzznukc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3urmafovy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3oxuiywwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmpsollg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3rnklvjdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrzlqahr.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3sdiahpul.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3exaknrsf.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3lqeidaoz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3erhphsip.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3kksbguhq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hssuskao.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3avwjvauq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3xqvxjmtz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3drneyuuc.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ziejuxkk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3tamyovew.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ezglpsia.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3slfhlpfo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3nunzesth.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qvnefbmi.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3nlundnjf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ewfhuwyr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hxawczbj.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3btjbfeqe.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3zxibcjuh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oplaeyeh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hzjzyvdy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fzvbizoz.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pztzwiuf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ucekuzma.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3qbpqcjjd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ymhxfwou.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ulidgtxm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3rjiwdlss.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3vexugqyv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3agsdrixs.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mquomvxo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3mlqgnsxz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3twcpsqvc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3vmyjrlyx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3wbynfclm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3ijvfavre.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3svykxbig.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dzispomz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sckxlhiz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3suheuibt.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3okrisrwk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3grcpicpx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vhifcfke.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dmvjwzaw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ogecdckw.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3notaazbm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3dmgafmnc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3tiqjebgi.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3deoyoxgf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3grtywvyg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3mwbgsdeu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3serfqoje.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yzrzzlfz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bdzruqqz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qbjlxmvx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vypxtpdb.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3szgknyyo.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qesktayx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3udcbxomf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ebdvuzfo.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ohxgqpor.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3obndqnvb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3muqandod.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ydgtrgcc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugzmutkj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3esjgrakd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3qsqknhcf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3scdazaik.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wmdmgyhk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3zhrithlr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hmqrncnv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xmfojtvk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xjuxjysu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwwsbnig.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tvdrftvu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbqigvpf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qzbkbavx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3vmxrafjt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3micjqagm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3idcdamir.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3cfyvpcjh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3zfnuxeqk.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3evgftyik.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3aqyjyaxh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wzlvzefs.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gnxzarxo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3neaiihvf.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3kofsxxzn.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3hquqqqaj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3dkkstdyr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kvjhhvlo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cxqgfccv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bgjxcchl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3unrlunfe.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pqvxpvmc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3vdcwqrtc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3htoskbrv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ayieqcmc.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3siyqzhxl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3rgigiois.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3yuawabbd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3cvrkczqd.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ykaekssk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3agovabxi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nnoprzln.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3gsvxtfno.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3prapaxlj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3cqvembri.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xoxmtqfr.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3necfukdv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3egvylyss.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3elraekag.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3umedqbdq.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ddjtohye.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wheyvlib.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oowldpgo.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3xzxohvjb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3uefopsxj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cyyfpyid.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rmvgiytb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tmrfunil.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3bsgxnyev.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wndyutky.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3zulwqfyv.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cvepsiua.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xuqxkbxi.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3duwoxpkg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3egjrpkgc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3seogcsce.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fwwabalv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3zwyjkguv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3cgqxnmtg.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3kikrwhxh.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ohruyvyf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3kotzcjkc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ewsrawlg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3wxenpwzl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3puldgwbs.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3azsnqmap.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3vuwkjpga.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3yqhdunpb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3sybqucrq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vlrcujoz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3lahpolnf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zokovjaw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qbxkoswv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cdbihtha.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kqlrcfdc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3znqmmccs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yzxwffkb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zngtthnp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xsnfwgqt.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3aafhgloo.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3whjledqy.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3upeyrwnc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xwssxpnm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bwiqqmew.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3hjeydndw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3xwmefzhl.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3rsyjdaph.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3dwqdrfgp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3tumuuhio.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jxvriwst.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3apqokote.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3egfnofhh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3eqgobtcf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3xrxdeibb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3djyloxtj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ytawyjyh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3uprshzjl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3mnlajgtw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3olxfsrwt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3udxrbbyh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3dsuexbgz.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zwjthwwb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ojyrstff.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wcexumih.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3yovrqajd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3eerkdpaq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3rhguuois.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3msuloyke.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rajnvvjh.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wbgiavfi.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cgkffnux.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aobiflcb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wnoxjvkm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xbrndwde.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3dpmtvcqq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3eiiohvce.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hzkbadqx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rvcyxtjv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3lxtheero.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dttgsooc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wdlhefvz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3agbsmlhq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3drvfehub.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3zxmjumek.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cttvklyj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ymfnslmi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ptgolgpq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3naknumlo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3khgjyodn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ucipgvcn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gxumgfup.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ixrbxbui.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3exfhwwjc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3rpomlrnr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3vcpomwlf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3mydhbcuh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3txhmcsdx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gmeumcza.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3jkobojzs.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3hifrzjkk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3qzrabslb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pcdwnjtn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mzhxfjmk.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3pyvgsjuq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3vnndwenv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hxrnbgvy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3huvsrzzt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3jgfbuzcc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dplvhxoi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3mbboasux.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jtfrpzel.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qjgafsqe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3trterjsj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3gfwschva.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3wmnnwvlx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3wmfrcyrn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wcnaotgo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3kivvbxcx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3wlavakma.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3wadujaza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tieutfzv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3dveankfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkrhqwkf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3mfizwhqc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3bzoidolc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycodbtle.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ouxjbaxq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qdsftrkd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xkpatgbk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3opqctmzm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3wgaqgezn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lmzodqna.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3esadillf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3umhpdwke.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkpsamwl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pfwaojyt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cjwricht.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gidagvqj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3luqvbqvi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3wpwmsuwn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dvsnvjgy.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3sxhieaoj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3pfploncv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wznyfund.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lfoicqso.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3azskwycw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qieemcyg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xgusnrzg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3iktykqma.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cykvgqoj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wutiylcm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3goslobcs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhibdrya.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kmykjjzq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ghdwpnov.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3anontnko.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3htxouzvt.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3gznxaszf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjaapufh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3decfwomf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3lulxzjdm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxuwalvz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mcnbywkb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xjebxiip.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3krcrfvlz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3szgeqacb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3kimmgelq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzohmqkh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3kebhsbeu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wkvzxufj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3wyalvtqd.html


<!-- 参考信息 -->