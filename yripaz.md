代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oauypoke.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zdkjtrsa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vwtbxpeo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2myooramn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wmyywmqz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2venoolpl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sddjlrhb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pxkptebl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mwgdhafv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cvicjqxf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kbfhujgo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oavgaizm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnhpfvlv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2szqasegb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzhgrptz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2auiwqhta.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2iriyfqkn.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2jywiulth.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pdgzptoa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2tbvezzoy.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hmrcvzbl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2spcipmjn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2kzriahrp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qyxmuhbi.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2pezomqao.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2utfsofol.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2glztfecj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2aluqveex.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2twnpezzn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2esbsknzr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2vcuqnhtp.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2mmzqopms.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uewjlwso.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2zbdxqzeq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2rbotkijt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lptsyays.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hopgatvj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lrvztizw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fpeqfapj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2frvjxbed.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2brjuwcpk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dkcgnour.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jskfsykl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2pimfswjb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2cduaoita.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mpcvjchb.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2dutlixqs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2prmygevs.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2fdninick.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ibsgbrsb.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2umowzhke.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2xsfwatzh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2hwoyyjjt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fcwzrztk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nzkrbtpx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2katwwvbq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wbegnshk.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fjgnrria.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gxwzanbm.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pyxcpszz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wdyusyyj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2imbzavdu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nalfoyrs.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2coewhrwp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rzvfxnjv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hshksytw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jdetcotm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2wdrroamk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2fyohqzai.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xgfejibv.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2mayowasv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2rtpkatan.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2tnjciyou.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cbxtgnlq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2aumnybkh.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2bpvzqlvt.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2yzigiyve.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mzqjhyyz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2cgvsibpq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zrlzgsve.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2xnivdqsy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vszmdgxs.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2sdujodwq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sroonzex.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hsxuvpew.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2swceyfsz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2prwxhzem.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qwmblqgi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2etzjagpg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pxiwtbfh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ylrjtnsp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wlfnwzse.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xsehqbny.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2pdaxqrsk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2vnjltwgd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dfksfvpu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2orygxdkq.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2jvdugmut.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ljyuauls.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2pldcmxxg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fqueoeuf.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gytjpvpm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ziygggbd.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2aiukduaw.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2qgzmsggf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2vdkvfjki.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2kqvpguac.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2owlahinv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qnzjwfiy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hazidypz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ylnnxzrc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gbklkzpn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hdrmlxuz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ksdwzjxr.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ssawtxhs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2vxclmkcn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ftsgivou.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zkfndaae.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2kmhgaucm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mmbtgeli.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2hmmyeymx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2brmggoja.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2tuvvaipa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2resdggkf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dugngeji.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wjqhvowf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xxyvwehc.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xjsercaa.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nymnearh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ttbuvugo.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qkclhovg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zokprxql.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2tqnoiwwd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2umuhyxen.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ysysyhky.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jlvbagxb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2efkkryaf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2lzvprgou.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mujcsjxa.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2uuxkndqf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ycjbguht.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nsdyvzeq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2larrfttq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gzreykjb.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ahqiddfc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ysbofhra.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2vdvllmmj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2rmhkrewk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2qlcspzhu.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cqfsteqf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2jsocpzqv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2owmqnrgz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2abcpqqoa.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2xdpjypkg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2dstetoui.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2xogupnpb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2jdwzwoon.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pkvnjxev.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ylyfgrsb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ejxtuucl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hbyashvp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ntqzvnig.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rhimmfhw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qgndmbrj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oepeobas.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ctkglqoq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nrjgkgqw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vxoqllft.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hzqglofa.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ddytnjbw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bavlmtzm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rdfaxxej.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2frluawmo.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2wsbvjzbv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2zumotako.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2lcoczvlg.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2inijgocg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2jjionihg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2plpumiap.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2yvrhmygg.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2hfjbfugh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rtrmdgdb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2mmcyedon.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2plitjctt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fugjsupn.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2iycfmqqh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2xzqekxyw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2lueavsws.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2nuvaaklg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2xubkjhdu.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zqktljlb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2kltzprlg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2qvmjgilz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2hpffdzij.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2olblsjjr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2uaaviwbw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2mrlzpapu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hfovddyq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ncdmajmm.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vrnxdktn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xtmqoelf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jnlviodc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sdbzlotu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2wklrhghm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tsnazozb.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tuypfpba.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2tddmqsdc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2zotyzfrm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wlmootcz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2bxgditbq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2lgvwplqs.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jpzawaua.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uxrnuixa.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cravdcho.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2peflygmv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qenqoytv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jkijiwxc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2barmachv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hncmugod.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfmaoqsh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2prjztynb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2hohxjdov.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2xrxrejtz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2jgwskukp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2jlfqpzgh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pbmnhuta.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uwffoxjv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2frxtsekq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvowgvmx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2jwlhtqvn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2drwnysde.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qizakzft.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2jflhmsoj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2loictxwn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lxlxlvzn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ovofqnxt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zaoejbvb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gqehpfji.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ygldavdd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ktwafhgh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2cbrhgojz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2eyjvskuf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2dhphzcks.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2pibhkihd.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2uskzqgqe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2uslqxvrl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2mkfzzpbw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wdxybtqc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mfrkrqig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbagkckr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qlyntnsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtztyjcu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lefxervm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kqmqtves.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgpoyyne.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2prxdjcya.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jzcmvlpo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2feaaoyie.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2yshbufyc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kxsnftvs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hotcinhu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2bysfhhzd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2adjqyaat.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2grmmniae.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dcfdhgks.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rfqxsyff.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bjkryqke.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2swvhwdio.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2rjjbxnip.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jwufxmza.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qplhotms.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2qbcndysu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lorlfhzc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nefulmxw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofdxjmvj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqtadfzp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vpdghmfe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dvzorbkm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2eoomtiuv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wbnsgepa.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fmvbfqzu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wohkhktl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbhhucai.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wcuidxbr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2dbbmeadm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2uwzhfiou.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gfbzfwbm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqeqoaag.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zvvyceil.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2subliizf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2erbjsejm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2peiossdf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zppqtohz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqlrzayo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wizxeaip.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2srtdxouc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2lfakivau.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2oarxumji.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ayipynan.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntnxlrns.html


<!-- 参考信息 -->