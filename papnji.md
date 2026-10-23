代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ttqisugb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ojrqzznh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qhzddbzb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3avgrpdvo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zeryabpc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3lsxvxjnr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lfdzifig.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vnmhksvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcbztogc.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3jgyrgihm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvrdhofc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xriawcyb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3maaavwnz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3kshgtcsl.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wgqilkgr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ajhfydrh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ilbvsbij.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3dbgwefpf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3imzgtwhv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ikxwvjlf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3mkblkwtb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ixyixmrx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kaeztpnl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gefizzba.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3scpxhzkj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fmnpqstc.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3cafypttm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3vsdwnbhd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hpeecvch.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3nlwbqdwh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3cijsmazo.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aifkbapv.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ixzgcgog.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3htarqlwa.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3awwmuskp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ntkhxggr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3kboefaby.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vklcndwk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3vtfaefur.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3sfxdzoym.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxsgxodj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3cwwcmpfg.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gafekchu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3lqabwgec.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3skxpqmhl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3fhlvjqop.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3jbimzoqm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3wbhfaedj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3zzlsmbxw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cbkajqwp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ledlilvu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zisbjsns.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ocdjobol.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rwepjoqz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jxozbnjc.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3augrekwk.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3agjexltp.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ivckhxqb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3omrqlswd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3dedcxkxr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xdyqobij.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3prdhldxl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3htgstxag.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3bthpijem.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jwuluwwn.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gifivwfo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nmzvcpug.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3lscdpgzv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3khbblssi.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3trvogcko.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3zqyreart.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3hpawggxr.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3yppgizve.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hyjatnea.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3cnxdmdsf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fsmnjozy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3heezqahw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hhljuswl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3lzspzzlm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mswluccl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3avrjfjeq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3rrndodcr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3frydunrw.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tfihdoey.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nmpzfnjc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3brjrvfum.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fqxyajtx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xlldoeuc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncmorqfr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3lnndgwas.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3deggbbkr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dxyitfki.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3bjgzlphy.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3yrdlnjtm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3sskwmjlc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wdeoqipi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3iwsmhiag.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ypdkgjpy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ynebrnrt.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3oeyihdjc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3grcqgxyu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3rljmtibo.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cyqlhhfy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3omudhqqm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3obunawkv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dfwuozuw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ihdmlmya.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3nifongcc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3renaxlah.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3udjnqprq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3shzbcpcz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ammyhazf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3cxnucsyz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3deudasst.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ueqmeyoz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ypmhuakk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3plillana.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3whvfxsel.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3muijymtv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3trewvbju.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mgbktqjw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3msbkfncz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mrcovqgw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kfykufoe.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ipqcdjfs.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jbcwwuvp.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fduoupcy.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ihfneslq.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3jfbdsspl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3mymrmpdg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vmajhlmx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3deevvprk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3sowfrrlu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3blgmizcw.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kzusztjg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3uoyifgxr.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3iivcwnxm.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gkjwmrte.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3bhpihuez.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vqtjhzku.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jqatjdro.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qzahfcal.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3hobhyuzs.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3otxrreaq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jafylhrl.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3goqyghpa.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3nfyovrds.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ewutghol.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3jvtswhpm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ntfmmseo.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahlvsinz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukhoojwp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3qtwyxbwd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ysmvujxk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3osflqzqq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3lmbdpqee.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3raxccbow.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3etcvpmch.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rnztmeqw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xlabsngh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vpytsvpd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mizkipwv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fbkyakqm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wivbxvcj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3yqhncylb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cgnalzpy.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bqsqnhhb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3andqpidz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xsmtexao.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ifycmorr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3impuatec.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3wczndukw.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3zqfythzv.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3kekgqskl.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kwitcqaw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3vjyplzwe.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nicwinvi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3buwmzpzv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3zsypejuh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3idvxcbfa.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3srcwupvu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3khexufan.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xsfyliaj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ynyedrwr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ygvrlozh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3fsrgisvd.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hsllplkl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3lyqkxbzu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3jqwabkxf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3rgiwkhnq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3uhlruxas.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3xrxejbvd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3lrtvidnr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3izamfejr.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3busfpkwv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pafcgptx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ayfknlbm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ipytudct.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zksoviwy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3aqjccrvn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fsoawkks.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ygorjxyy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3zgfuoblj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3fhxwyaoq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zmqkcybt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3axwtgohy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfwjhndd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ynojvovk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3czttapop.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bzmlwjru.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vetutavj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3nhgaknwr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fcekvjgn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pyuuawbc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qjnllyuo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3etqejqoq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mitvjewy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ljstkkeh.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3zgekjfkn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3doxdizeh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3lgxaiewi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vxhlirsh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pidyitoj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3vooycfif.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mxvffedb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3mmzdpuez.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lvrknzfy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xvckhast.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3gmjhdhkp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wglmewyp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qhcimtdm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vqtsbatz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tlpgadta.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rklhkrif.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3sotgztfv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3fahhrzzd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3lzmulymg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3vunvpqbd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wohsfphr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3oypqnxeo.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3pcgepiii.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dzkmrrby.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3utnzcheh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vwdzcret.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qsktowoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ityiwydk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3eokujayq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyhbxhma.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3cfenjzvi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qrutytgs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnhfounm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ewlpugqp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ykkwijyn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bpxfrioc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3lowflxsq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3lhikeyal.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jxpcjnbi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ognzpheu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3nmpadsdo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3syzasfrh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3utpnkesi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wbeedpyl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qumcfjzf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3umvinwoi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3voessdkb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yewjaaak.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3amkhqsws.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dapvmncj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuhhvfoc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnkbubie.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pxnmhowr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3krvytwqa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3joxszssc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3icewdvne.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gafpphyb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ofptwssq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3suhqmhjm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3znykjpoy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jxwtauhh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmfdtsbb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3pvfcxono.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ljvvfygh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3jkabgqjw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngbrxvvb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3enpyckvd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3nwawtgwc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3whyoynoa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxtutmgu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gggxuvcz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3smnytaxv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3imwjdrha.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3zjefzmkp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3kejafjoh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ixnxbjye.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3neocygsj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbtlhndl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3aflvkjge.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gaialkey.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3eovqzueo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3uotltovc.html


<!-- 参考信息 -->