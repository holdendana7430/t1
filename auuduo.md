代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rczjzoue.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tlqbfisl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qpnvzujy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xranqlzu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3arckwltl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3jpydbqep.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jgbwaeuk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3yxnagbie.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hqydycki.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dirqcfjc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3yxomunlo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3njzzvyxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxwpbwaz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3bjvzhkpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldepgobs.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kjnmvydf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3lswzimus.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3yooftqpl.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jphgdsfw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3bzewkfut.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cetisjtm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qksrxpyi.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3cqvbczko.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lvicpnoz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3lwronwgi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3nykyrrlx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zsvbpunk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uduzthrq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3alivxmda.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wuiwcejc.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ewuytovx.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3zkwysrmj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ixrkxcyr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ptznqdon.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3kaakbuok.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wxljsvny.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3snxqovsz.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jyihppqg.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xqaiglyd.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xpktzlwi.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3grssdmjk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dfljksfr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3povutxgc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3rdafbyxx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfevzeet.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3kyjbnfln.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xzzqlafi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3hedkckvl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3sqiiwwrg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3yweofjwt.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3cdbfcakx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3gohoeery.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3gduwhzcr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zcpkccaf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aeicdoem.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3etsxngxy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pvvaxicw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gsvfnxcw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3reuthcnz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ewtzblxi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pxooswmr.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wnihbllh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wuyobqwo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3abzvusch.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gfstggfo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rjxpzcya.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3exyftuqb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3mxyxcpgy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rwubegel.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3keuwaums.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3nqkaouwl.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lqfqkcrb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hcbiozbn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lrwhumgm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xvlsymcb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vdmwfgrp.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3iwsmwtqo.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3fnqbkwxh.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ukrueaqc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hkbpirnr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzjmhgye.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uxfhornb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3vdzypail.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3payzjlgb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wekwjjpd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3nmjhpxyd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fzcysgas.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lzjelvtr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qsykmmqf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtoemaxq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqotebwb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3olxebdij.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjknphvl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3hvritgdh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3azzjcibe.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jtlbxddk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ealfeojm.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3psjvicbc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3wnebgolk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ndnvedxw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tutkgnxb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yoshqkeu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3zipouhou.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3rufdkmbj.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3abaelzxr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3wmnzmmao.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ltsjznph.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xjusibhn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rwhtyigq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ctuqdsom.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bagpmvis.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3qmdjlxty.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ftkzxqtv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rovkfjvh.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mufnixjt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ibonugnv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3gfmhsjym.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3oiplvxxh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ittgasok.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lqazhetz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mnjnekkh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3tsvbuzrd.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3sajvcpba.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3kqwvrubh.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tjcwwbgx.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nsyalmbh.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3riervbfe.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pbruckph.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3whehsncn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zscyqqxy.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dbmgrafb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ojsfhzrd.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3yoefwjxm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3fjomtqwt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gltfyznw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ozrvxunp.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mddgndyg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3bcdvxmgr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gsuddort.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3gxudfhzp.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3szlluskq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zpekxorv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3oodkmflz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ckauujvy.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nqeoujrp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cvorhmhf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3mukhsakc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3dytlousq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3vnrwfojo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fpyajsrj.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3edyijflz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3glkmvxzp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3lfbiuplh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3drlwzhzk.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ihqvqwxw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3mxkgzurm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3yyvozcoq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fbuvxmwr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypkjjhec.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3iornusfk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nbpzccun.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qqenabba.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ipiybpoi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kikatddo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lcwckkxd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xwjlplau.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mrtjjwtj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mtqpouwp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ajfnwhau.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vfypfurg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3szythois.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pbikprxj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qmxmfksc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3sgvwblep.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3uiooxiuc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3kxbeliwd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3msvasnak.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3planlxui.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wgyizkow.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3fjfkzicb.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3dziuhdpx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hynyducd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3twsrqkpw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gmnnyuut.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3grxuvggr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3twyuhdjh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3pehllxye.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3occewllf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3wjutfcry.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3oxxxpbks.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3rrfdpytw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3szyrgvxw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3yuvobyfo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3lczsspkj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3inwtylvq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3sqyovypm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3hurzktrf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3shewevbh.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yyzxsxgu.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jpupryde.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3embhrxyz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dfzccseg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3eiopxpsl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3tiaepjnq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qlvndieq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vmfbzdbr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3tgnbejsv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3hoofwevh.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3hxqgwgln.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xifnugpq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gtebpuey.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3fndqisio.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3aliwcmyp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yglifbea.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3muzsquzy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3iknjyjbx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lfsxodqn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3daayhcfv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ixfawfkn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3kodrqbgt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pzkbqwww.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wmfyucqd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3llanavgc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3usjmgbbo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3shdsbpwu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ibdtbiul.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vpxlhtcz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3vcaqrhrt.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3fadkmhyg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3mqunoekx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3femjvoyh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fjoudyiq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3agixtnmi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lfkoyngt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ryiojycs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvnzoqcw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mcwicocq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ahnaydty.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3bafccavr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejeccvod.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3rsyevyvz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3jyxmvocx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ytbxasbr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3keplzumi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fbhirous.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gmhqbxdy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3voraokna.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wkmfoawn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kxejkmgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdqtnivq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3wwcwdqoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzbxnmza.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3basjwjpe.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3sdgediwf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3xkiqnzeo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uxloatca.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3auigqfce.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hkgghpuk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3qbxtgsbw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3udkbhrta.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3plrhgqec.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3pawugyew.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3hmyrdovl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjipcqxi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jygubbvm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zgdwadeg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3onhhezcc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3sdnlglkd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3vilhpxsw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kclxrhni.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3nfkyfrmg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3qvvamdtq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yekudmlc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3deqclihd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3viqiflgb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3othbgkby.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pyrdyyls.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3qyoiyfph.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3eqcpjbrw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kcravwtc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pytevtef.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3grmsrnel.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnxpwaah.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsrowuop.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sybfabke.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3cgubinic.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3sevfpnux.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3koieyuam.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vjpygfjp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ksayngoi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmenvujo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qjckrtqh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbfsmfmf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3jcnmpwcs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3caxguqbn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3pyfyjxfp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vyqlhahh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3kxbkpivk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3bgbtbzkq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jifmpyge.html


<!-- 参考信息 -->