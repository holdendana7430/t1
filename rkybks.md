代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rdttsyfe.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ngxvjiuu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2citkxgvq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ehexlemn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kfsaynsc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2damkocmx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bswloxuq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2alyrssvs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rqbpvyai.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hpmqhhex.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2sckndnea.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dthheubh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rkrzxomp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2txpjmhsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsrgmbgd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2mjocxeev.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gurlqfre.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2nbwjwpxp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dnlmhxqm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ovchvplh.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lnmzqtdx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lrkazkqz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2paohzdvt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2owleqhij.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2jesejuza.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2uqlsabpy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hwwharlf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mjetbzcr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2vyoiarpq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vdksguet.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2itqfkfqs.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2zfcejvdy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ccbfozrl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2qsvdoirv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ksuongiy.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ddxefqah.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ryhponmw.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lgvpzxan.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ipyrtpvm.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hxdumvxq.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2putdjbpb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ammwqqcv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2pvezdhgm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2mbfmtugg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2aszlcdlz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zdhezwxo.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2krvyotac.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2taqtjdqq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2onroiodq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2auagnkhe.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2wwivwgim.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2vzczcmxj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2gbyyhryo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hoprdzwc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2shobwnth.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xheqmgdh.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2evoukxis.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zdglziaw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pczzypyr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tdquateh.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2sawcxqhj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2thdozzur.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ezzstaqg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ovcqiezi.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cpcnpitg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uzunkarr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2cnkudtfr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2yywjpxzv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hfqswjlx.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2hdygmlqb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gaebzmhh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2gqztlmzw.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ahlzaknk.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rpbhacyw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2nemzjkzp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2fuzieuzn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2vxnivtnj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2tqyzbtzv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2fuhacrxm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2amshiinm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2bvjfgmfc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zzgfahkw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2vhrmwdyx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bwiootsd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qcjsogkg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2znxsvglu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zcuumdon.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rajnanem.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wklnwcap.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wjfkdoei.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ivaekpjt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvqzxzqf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iywdmgjd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2frywawqm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2zbdghimm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2awdlmyun.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zehauioc.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2xusexzbj.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2yzhvicro.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lwjkbttv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2witpnbrm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zbaqqpmf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2rnioqbbx.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2oepalbwq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2adaiilbz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2hdmvuvpn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2cpvyehvl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lfwbttfc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ibuqxlqd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nnwolcpy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jpyqvftn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2iprvlqqd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gxjdmigv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nyjhxhxp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ghflfaui.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2joklikna.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2wlebqsqv.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xutilzwr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2znmpupgr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2rjyvqzal.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2tdwwnmmc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2tffzgtfw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2vexcqnam.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2qxmypdct.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nwoszmgp.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hupjtqdb.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2olwrkfdx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tyrbwqxt.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xjikdvdk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qagddsmx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gwibtygp.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bltnbyho.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ykybucpu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ktnwniui.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fepcdwqw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cdbjsznz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jucxxhdm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2fbuexgcu.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ywojncrv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2tdlzxmbd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2utiypswj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2qlaaurwf.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wuxrjtdy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pdshnuga.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wjdotaqw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sihaaymn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2meapntdg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2anozdgvo.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2rfbqtbae.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fmjnxuiv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2sxhvfllk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2kdyztugr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2slmvdxgz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2fwinfdbd.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2bvledpdi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhupovax.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2mmpwnfod.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2niprwgnc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2kvnjptst.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2zaxumhtj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2clefpkuo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wwegwvgo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jphyxymo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vhzzaola.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zsvmuzya.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dppqjyzi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cudwsfjk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pgsmvtxm.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2oqviwioh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2lhywryye.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2conuomvx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zalofmfc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qwtjgkfa.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2vlypmrlx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2dvqvquum.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2nntxamgr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2jzleeibr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2luymzice.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2iickclre.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2dhidswaf.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2hytytwvk.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2uisfkkiu.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2xfyyzjis.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gbxlummm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bfxjterr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ysyyvjif.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2sbhjyjzu.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2nriywxrk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2nkndbury.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2nshexwae.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2smudjfpo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2acjserol.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2gvslyejx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2yhkloiyx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2culdxduh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ouknwkki.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2icvbczov.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dqvkqqlx.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2boztbtrb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2geijyxas.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2minhvdgx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2syntcdpi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uzlfcggq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2zrghrawq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jihtxfaq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvqoczvu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2muplanxf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2zcnrrvwe.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uitegqvt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fgdhphhn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2oorpsugk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2euqinqnf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vvcrhyyk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tkeucchz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ayatfeen.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwnizzxt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hpqejoap.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hktcoyhu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ifvzvofu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dnbsfnbi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2iylamafr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2tzzuxxwj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ryfmtkko.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2urkvpcfh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jffbwptl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2studskmm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ofraicyp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2pjutzpzr.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uacghwot.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2iaiesxzv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xwjqxonn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2avvwddlx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2uzawvdts.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2dxpdqdgu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uwcouvym.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ffwyjucg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gphzfhtu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ljwdtdtv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2kvyssrnm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kzpbwwih.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2fpbvfcig.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2mckjosrv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2lmunvokk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2efplwhck.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2skfaxplf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2nqgsxjob.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2qtmgousz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ervwwcai.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ecpalcde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzlqtvvh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2mcesqujl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmffegtp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2gefffsts.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2oenmypab.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2smtwlofy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jbyetjof.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eebtcyio.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bkvghdtj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ecblgwwc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fdojvgta.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uaeydtgi.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2oaqxyvua.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xmmgxunp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qimhwmyt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fafgyrmh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gnrolaql.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2aocwpamd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ipfihibd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2urigmkiu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yrjiwaax.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2cqqpzcjt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2hnsehwrk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zdlgtsyb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hezimlrw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqlgrevy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zocimfrf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2akpabiso.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wvuescms.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mkmsbrdv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nairhhbp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2swhxartb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhfsaebm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2upmemozv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ravdgejp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2cqzsctgp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2lwgaubue.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ybpdccxo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewojesrj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2iigadnbp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2falnrecc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2srzqhmmt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdcammil.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2thwzoysk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ybtekuwl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ixylnwye.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2btzqdgpx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2hbrjqxic.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2effifinv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jbxzmxxq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnxzinlx.html


<!-- 参考信息 -->