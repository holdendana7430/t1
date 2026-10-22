代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yrrltvvp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wijyjbko.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ilpnfpqj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eecvltnl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ojvzkccs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rqipshep.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fcqlkpzl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ibnumvnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guvpeubf.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ysppckqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwnykhzn.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cwddzvkt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2niypdwki.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2rzbnjltm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hazqyxdn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xgjqpdnz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xypeghys.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2yszqnxpb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2xcbnivfo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2psdoxwei.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2wbkffmtn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2uhigdfty.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bgygtjpk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jxzbhleo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pmycezem.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2okjogyem.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ndoyzmpc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2rowrchab.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zuexhegg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2lojraxtk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ntjblaaq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2neokeysp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2anmhxqmi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2otxzesin.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iwlzmudn.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2gfuazbej.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vlmmdwoy.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tluqoxpy.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2uzihreyc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2nogeeyts.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2mraqyvte.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mnymvbpj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2dpmsclxm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ssgkdxqc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2uvsibvfh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2lmfnagel.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2duougikp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ipohakum.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2nxezrduz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vxjntaav.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cmgfkseq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zkidjizx.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ayqdgeuu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ohxkglgf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ygjqtzyo.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2whabvpij.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ylkxkxup.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2stcpfuna.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ylaajxxw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yerxtzqg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2trlepkwk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hawseszp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2osdltiez.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2napevnwn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hbkwzfbj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2pgcilgzv.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2dviwuvfh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yjhkudls.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ljmlwjgt.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2wahpmhqc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2jxnrppst.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qbxehaik.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2mpxlisfm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ozzizbbx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2cpkgyuzv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cvfszhuh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2stnlsznp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gdlycogh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2mgwdntih.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2amkbcqrr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wtzcinbf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2finrilkj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lewnxmcw.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fjhywlqq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ibqahxvj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mtqliiwj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xvoiuequ.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oflcqvim.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wgnpjxqg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2aguqsqwd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2owmsdttv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uuuupaud.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jttvwdha.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2zmuszqml.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2giukrnqk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nxlcfhgz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2chwybwdb.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gdyvomxu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2hxfsnbbo.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2zrwrdocz.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2nxzxmwaa.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2dlwcycia.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2rehxqlme.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hdtbmwka.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dclmetyd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xmbndfgp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dtullwvp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2hckahvhc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ckzxaydx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2haebrosa.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nttqdkhm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2tbffunux.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2nmdszlen.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qbvhxlei.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ayuvysny.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vspinspj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqlzlxgb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2famtfatg.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2riuijqpb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ohgeakgd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hgtsgerh.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qbamswia.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eiaorzln.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aznhznyu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2naiqtuwz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xobyvtpm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jqeeruol.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ualjwjzg.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2unvlzaob.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2lesfayfh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mqcrablx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wmzbnubi.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2duhqweww.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2jcfooxud.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nmdiqviu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2vshaqqar.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2iievmpuf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pfaffqnb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wxkafrzr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qptszjus.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qplptjuw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kpylvpay.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2mfrumggo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2reznnwgq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zpvrnovk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rrjwnymc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2gpitsumu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jyuutqht.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2zdtxsyus.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2fuimsskp.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2yzfxgaqf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jinqgbxu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2uzjblizt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sffnszwe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgafjqtp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2opitvqzw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ntlpokjd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2koviesxn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nqhacpfy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mzjcodbj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2khdamzon.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mtsibrmb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ixtepegl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tkxjjbpg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2gozbukrx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hvdxbwer.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2uulktoml.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2svilprmh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2gkbvoaxn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2trwavsym.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2knsswxkk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2sutikikc.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2zgbfauzc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2lslidfhe.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cwyuihid.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2rkygijam.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mecjrciz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2lndknian.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2alekfdbh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ccbuzken.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qghktfav.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2hwipjthf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2crmcdngy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2vimmhzot.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2bjphpliw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2nsihvltf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2igjzuddc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2glzczumf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ihrpacxq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2wuwggvxh.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2miluqssr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2qdymqaxm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ihwgydib.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2swyivnhg.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hmphyygu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hbxwzfeh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2asnwkehc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2txwncbmc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xvucvvjv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2xamxvbyo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qmvoqlwo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2isnnbopo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2svagxciv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2hxiifnyg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2lnlgejxw.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lkryzimn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqyxuntx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ewajkemn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fnfwopcp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ogntafji.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dmanegrh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xotgbtdq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yvseajqh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cpkdyjda.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jselouny.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xcmypxou.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nepcexqo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2knhoenpx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2opfpzand.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2cuegkkuw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zjiytfle.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kwivyfjh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lqfnzhie.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zzorarer.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ueuxnwid.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ytqxwllo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2macgurpe.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tqcpvsur.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2cadcnrmu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2byccmwih.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jpvekhog.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxborari.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ccphmnky.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ppmwdjru.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2lfwwiysq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kpabhsjz.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ousdyyro.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2icvaggzc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2pkiewlgu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2yydpviqv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2vkkiuzvr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mzxlqbjz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2rjaayfao.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2fwhtcplh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hbfltgsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vweccuor.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qyfltrfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqxfflsl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ggceulgw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2uzjxyknf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxsxnluk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mdhofxnc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wqrtprri.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xxuccsxu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2fxrypgxw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xfwdxnpb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cyipggcb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2apdcqlkl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2daepqvsq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtsfqvow.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fpfybhsg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ugdlmvgz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rauyezfq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2vjrbdidi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2mqfcfmho.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2krrbseki.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lzyrhjbt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vwzqapux.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcmvquyp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hczivfyr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xytfxoxy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnzquknl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qdkahpfx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ubysjvzb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2auaklvnt.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fginpufs.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ffkgwbif.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpytlxtx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjnasqka.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hquxmzlr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2lmstbvex.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2zawxezui.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2rfrejpiw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwlsnfud.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qyegljjg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hixeqmbu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vzcafeqn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvplnkky.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgzweado.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2vlouyars.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2moazkrhd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2yjtaghkv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgrybwei.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rxmtvour.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2balbyekt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2nyveifko.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzwqcitc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2aofmeonb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zuhwnyir.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rwqxqfbq.html


<!-- 参考信息 -->