代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rngzrzfw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mdvsrwre.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iupdfxyv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hgqygaxv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2hxtrjnhs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2qeavuxtx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lpucmchu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cyphuinr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xagdvbkd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2amhqcrbr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gmwhqawq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2halqwphy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apgnesha.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2hufuojkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfbpghkl.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2uslglhum.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2wreqwbvl.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2frpwruug.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zwdzkxqu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2yvjcxjvl.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fjogltbe.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vimiwiee.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ghafhkye.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ynkounbt.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2axtxwxyt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2flqfgzgx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2oslsgjjt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xxeadrlo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ycwxnquf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qcwsnvcc.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2gervezny.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ywkruqff.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pnjuvcec.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2wssasruc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2yhabivho.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2agbkzdhj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2odmqziuh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qssvzpcn.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wggktmgi.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2yqjqiemi.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2osqjhwkp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2memgrimx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2hsiiwtuh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2qnplanip.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gclrhzod.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2wqjfkqrv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ugdzlhxy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2imoelnwi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2jocozscr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2amwstvkf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2jatufgqg.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2csisubnf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2wloqxbnt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2iczevvfc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2twfikmgd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sqqgnogx.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tohoplkx.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ycqjjtnr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xlteawul.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qjezgfsi.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pttizcsy.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2guccbvnt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2hlkitfdj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mvapsbvw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ldjmmaog.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ggodrgci.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ttocpifj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2hqxqfhoh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mfypflch.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aitndqjc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2dfkdrnrh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rhcgupfe.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ijoqfdyq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2efhitiyc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2clifuoxc.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mwsxjpno.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2vtzucmyk.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2msdvjnyt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2pkmqxnwa.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jvpfnktn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2upohyxcm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xdauamrr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2tpnjeftp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2chggeuns.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2raphfilo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2mdghybhm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nqxxxnrh.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2oxdamirf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzrwgimd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2numsycfd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmsbuqkp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzedjljv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jywhqanh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2nqgurodl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2nlxtwwxt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2etpvyppf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xcvwyymm.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2bdugtwox.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ocufinke.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zlnrsmyf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2spueklpu.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zopwxugc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2vwsypobi.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2fvgxpsts.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2mzmammgd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2zqoqbfgm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nefkemgq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xrzqgkur.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aytmeyiz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ddfhfgxh.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xneoovmf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2egcuweta.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kzpszgit.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2idkhpvxv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ilclkloi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2pbtkmjpk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2psvhsoxt.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2nwaevmls.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rgpxiftu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wnmmoguy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bogzgibf.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wvthxwdn.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2stwnvqln.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2rnfwwuld.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2apwlrptq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gmhemkyp.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2twvrmbgx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zmizmmze.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2weixbawk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ohwrllyz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ydkjtrds.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ybuxtngx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2veezkjjv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2cnzhpuhd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wknnjmeu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qjtkussk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rtfjwrgu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ixwsyibh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dgqwneqh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2uxzwdzdx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ccdansma.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ctvoyvgt.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2dgmziwxf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dotgwvts.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ybaiouns.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pogbrswa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2satqvmds.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ldokchmm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ssyrqxou.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2grwjzzma.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2xlnkyajh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2opyyjcth.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ysntnebc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2klgddoqt.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2bfgznwtv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2mxmhpmsc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2zwtbjgxt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ssgwdbyq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2fumzqdwe.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2fafwipgl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ozrmhbrr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dazmmwus.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jmusyxxp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2caczukeq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ucvmgdgf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xivivtah.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aasanagn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fckqgprn.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2awwohhye.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wplwaqhw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bpcvqmky.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2kzzsfzyy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eshioaox.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2mbdzsvme.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2haupwmea.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2leiqjkvs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2tqftensp.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2cygaupqj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2aslzemky.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2rpcqjeyb.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2zslujjie.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2sxenhzhf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mlftunjq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nucsbsut.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2uvzfrnjm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2capkvqfj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2hwqlggpy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2xpfqymst.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2eowougeh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2yornsgcg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kxvnbwxb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ppdldxyy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2dimeszmz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2uivcafkb.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2zfiiojxp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2axhgyppr.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2nzlgwnpg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2varpqmdd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdwwmfb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kdlhnxrr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hcnbwwhc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rwlhvgfs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cldminzu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ramyapab.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zkhxtoan.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2eifudzgf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2euhsoimp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ucscvljf.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wsbepffs.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2bjxeplcz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2vdrqmngt.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2yssqghmw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ukxadvnk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wclnlljd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2auojkgce.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2srzedgio.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wttxnoui.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kkpmvvga.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bcwlkrkt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2fpauhjev.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wbxvjcco.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2zusommjv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2cjpuboyu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2nfwgkanf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lkvwdkgg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hprnubzj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jdqlvrhu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2axzngsgh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ghbmtjbl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2jzlmxybl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ldjtqedo.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gomqxyca.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2fiyelosu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdnruzkw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rxvufcer.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dgpixvbv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xtimfpni.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bpxmkskq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ycwjqkde.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpptzwii.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tpuufeou.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hvyhqqxx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2wtwmsgjd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2gwefqxtp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2mvoysryp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hpxcoiyy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2oijhpdwm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2mdrqxzeg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ucuwffmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nsoewlpg.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2uzdskjqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrgehllw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lafbxzhf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ecbhcetx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2grtthhxp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ubcptsrw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wzqrngzy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bhonwuhu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zzryzysc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wbfnikhl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wjhbgkur.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2soettowu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ndcwclzm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bohdjvzz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ufmkkwpr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kbcqcdni.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2paluzyco.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2nyhcefgo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ddsfjtof.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2eeycdhaq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2slbpxufn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xfukqlzx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovqkzcdn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2crrfjbfn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dpmjavbz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jdvecchz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zxjbswsc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2buotzchp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2clznijgn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lgvxilgg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2jtypmqwx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vphakium.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2berzihnk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyansesu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2evzwrgzg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2qgekwogv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2webkrtiu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjoteqey.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kzojhege.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2lyvwmsii.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdlwjzxo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvnnkqzw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ywnibnbv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gxslcida.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ttjjjztp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2igjcgpzf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2odlylhnu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ouzcrxjj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wxxliztn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2krfnjqxn.html


<!-- 参考信息 -->