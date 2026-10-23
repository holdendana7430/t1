代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jfebzttu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uvfowuec.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bntwzrzx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lyfheudq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3cbgfwtis.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zrnmcoar.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wtmvmvev.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3dkkqzplz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tittqxgg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zstbvhsd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jdplmtxy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yolbbmng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpzloghm.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3bqaxqaeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvekzmvv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nspvtrnt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zhsxelod.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3kuubaycb.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pckcuyxo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3rvffilne.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nxbnqmok.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3etqbkpqi.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3djvacitx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pnbopzci.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3yazcrrqq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3akhhdrdu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nozohifk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wjrapuoj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tsntauag.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wnkxjfzz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3mcviuyho.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3rolyuxta.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kzjreksj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ikuhvucu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3veqimjhg.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ageoukdn.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pdkodjxg.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nuissanj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ajguqygl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3wgjocmrv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3sfpsszll.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qkacvmgd.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3etpxucqz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3dphkujkt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3twlbmixm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sgkolsnf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ottixaqo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3bymjfgup.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3yzzhkgkl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3vfyqgljz.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3yseifeft.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3hxuwovpi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3zkmehets.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cdokdycf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xgmyucme.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3darkjlxh.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3beypwclp.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3phokuzng.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ocyahsuq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bqeomsmj.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3khgeszmb.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hkkgvtdj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3znvytdpx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gxmzsybk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fxxbnyjf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tvdtinvt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tqbfpmqn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3zefjdmhn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dauaagov.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3zeqakjsx.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rsnivwpp.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lkokjsgt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3qnomxzhj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3itkyeoov.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kfhumnnj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lcpgbymn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3cdizmjah.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3qoaxrjzo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ffnirqtc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3knjkdxqg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3myhbilci.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dbshoxny.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3tagfowio.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3efvuaxnq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3goywuido.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3jqbuymda.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3upcgeqht.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3flljbirg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tullaxdr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3syuwykjn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jtdahlgr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wdeowvxc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oiqmnfan.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3wwydmxkw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ykuyxchw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ohavrlng.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3mdmkxfti.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3sdcckzzx.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3inltrnxh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vbdshupm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3snkjkvcw.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ktwevula.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3hdbmcvfw.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3aguthnhs.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3vxhomzju.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3gdssryiy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3akwyrsyk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ybjjicnb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3duldggsn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tgtmyfhp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qsxgqyqf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ysfotbzg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gpybqjxl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gbatdpuv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3tvtlqyny.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3opdvtzve.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3mpixmmba.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3odczujpd.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3pvbqgggm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3qnmvqteq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ayexviat.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3iqwywhag.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3rvitteyp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3gxbocbge.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3neiruvzb.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tqayrpnb.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3brklqqds.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3biffsfvp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pctmutmz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nvroeleb.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3spttxnka.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3csbnydqm.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3pjxjudzn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3bcmdmikc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jqccdnuy.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3itfhhvaj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ouzixxhu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3txevwinq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hmcflama.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3mrubcawk.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rootyawf.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3vzkxkfcj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3phyqwxnh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ewgfgnra.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3asxzyrvf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hptjqjew.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3azurbjbg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3vflvjlvk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ifbejgbw.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gwejecae.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3izrxlllo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ieiabtri.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3bqgphuwp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3csxrickw.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmquzxym.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aehfuedc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3rbziawfc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3nvqjrdhr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hrtktncl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3jrgpddxt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uszcwkvg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pqxmzeyv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3epevvyoq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fqkbyiud.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mrpxsici.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3veotfqbx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xalusbzu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hbkvypua.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ebhinemh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3sadzfhet.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ifaaoznw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wjsnszpu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jcioepxt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3auhrfdwc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3akbuviyh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3fjnvemvd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3bbtistnz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3oqpmptae.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ldtvnshm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3xatglnoc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3dpvfgwlk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3zrzkqufc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3xmfgclri.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3afatoisv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jvshetbd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3kgsopxvs.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3tszoircj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ptkqcsyh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3zbfcxndw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3mbjveapi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bxivrswd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3pouofaol.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3cefgvedf.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3bvtsxgfz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3bsrynkzk.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3gnldicul.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ppngznss.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tsppkoyq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3facjfczu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gvhczxbd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ibbvpxsm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bcwzsjmk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bkcbwzkd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ktxsjzpd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pzqhrphx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxqojehd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3cyfkzaxh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3xdymkuzd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3suifjhnq.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ufrurcqg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3evgukque.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3cttswgbc.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nwzymdpa.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3glrkukar.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3teeltbya.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vxxduxiu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ysfivxnl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3icvzzksm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hnlfnmtk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3raakhqje.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wchapdlq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3qkprvdgx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3dxboufej.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3mqqqzkfi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3byuilxma.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tteuefou.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wmmamhwk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fppkdrqi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3rynlnrrs.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3rzwbtcbu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cqidncvi.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3stgpevsw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3xvkbyztn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqabyegv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wkkjetim.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hvqvpomq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3hgbhzoao.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lginjxjj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3autameor.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3tkovtehp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3byfxizyd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3waehmhbd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3mpcdpkvg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3qqposizr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ulrmbpxi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cenrqhhe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3yubmqvck.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3phlkxvyk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3knxidjae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfwupidc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3gzituxno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjerqgeg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ldrdzntg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3csbkyxyf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiagfwkl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zyyfwzzo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zmidrtmc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mxqxobtc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3cfdmajqu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xrriyaxc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hefcpvtv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3auzwjjiu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3vichsfwx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwvbuzgl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rejwqnbg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cuzngdoh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ccwzbhgg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wftzcxig.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3dxqlnwvn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ijkesoir.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ybtnxezp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3zzqpagmh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3elcxonid.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tedmsjwc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdtzkenf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ruialysy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3psnvjqnm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ykrqwpbe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pngwjyqo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ralvhcia.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lwmasdtq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlxiwlnm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbmtkhov.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bzdjytkg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpytyyet.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3sgtlgsts.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vybyocmz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3obnvgnni.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fklihkmp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jfxxppbn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3znhimojf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nltvylka.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3chikrbct.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhtvitgi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uyhkpfut.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3sbetmtcv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhpzisrk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3szuzvkiv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3mjdrxgar.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3flqxggda.html


<!-- 参考信息 -->