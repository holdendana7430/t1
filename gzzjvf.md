代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tgtomsvz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sltbgycp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cilmzbiv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3gjvkaycr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wfuvfoph.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3tmiuhdqi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vyoqnzlh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gnhywzel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlvmxspo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3wowxoany.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgluzvnj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3vyzgacmj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3bnejeqey.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3tycnjpuf.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vrmhtpxt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3acgqtefu.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uleftuay.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3lkduhtoc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3gvzthxtw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lhnfkrgp.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3omaghpma.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3hszweaaf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nyqrwarc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bnpustae.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3olrzlhct.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pdbiguwd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3syaequyb.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3cxoxtuxs.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yynwhhua.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3nejvlqan.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3nckpskxw.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jxicbvqj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3egllcxvu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bwfnjvak.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rzqmmpgl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ltcvdoyv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wnyazahu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3awssdjjs.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ekyuocjv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3qvrqnbyk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bjjilgrp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sdpvgqch.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wlzxfrpw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3qonlimgu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3oelgjwpz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3lciktoue.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3pjsjfcsy.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3tgwsnzri.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3hlukynfn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ffywyduf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ziylgqwr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tulzleox.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3twpzjjtk.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hyyigfca.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pbnvtxlc.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bitjeaan.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hhyjlkrv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wsbdzkct.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qzokydvl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fedjqchm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ybasjwdq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zyhpwkhe.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3pytfpwok.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3dujivkti.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xheoenep.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3iiztosnp.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ugrfubsg.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hbciuivz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xjctxwjb.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3jxztrwez.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hbuayibf.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3wujtopvm.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3kthvvrfn.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3duedzbfn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3cezvahvw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3eknccfkm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3pephcvgr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jdqxpuxa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ddgfivwz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kjsucihi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kqmbbonh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3vgmkoyca.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nvowssap.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xpyqbpgw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dzfjpfsb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bthgbljq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3upcvideb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zpcbuitj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dehlddrg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3xohrblzv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3zdpzwwxc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nziivjxf.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3fsyicuqp.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ufzxanwv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3efmjaszs.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fisnoxue.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3snnnvszx.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3alrtsdhv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3dxwchzgm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3dgnqyyyy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3glyyslaw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3yzactexj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3gywuisrm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ulgidbas.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3eihvbune.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3znacxqag.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dtirhmqt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3gazmhlox.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xklsclqb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3aoxkkneo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ekzljhhf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3aimygbos.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3asmeewbj.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ysbkwixg.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fjgtynar.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3csuwgyrz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sbwxbxfu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3xntodcft.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3axaoltvi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ivxfsizg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cynoimir.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xsprcasm.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3klwamves.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zehnbmhl.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3shguwijt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cattrmbg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3okjbvgqp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fcyktrqs.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3srhhsyxj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3aigsylbu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lbyacqry.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lubftoab.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3snegzqdj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3dkznymks.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qrceasvn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3hftdlbau.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xxdfsdyt.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mcckfziq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3khujkhvw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fzwvjdnp.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cmjftsgn.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pbjkjrpr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3qnnwccly.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3skrugqbj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qgfbunnr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tjkeqezk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3jdtmammp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3fewadnct.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ocoefanw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3btixdqcx.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3isoyqjdj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tivrybiu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3btfajdrq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jdgnjqnp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3pzbxknpe.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3tcsyngzy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mtxodmgv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tuiaipba.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nsnsbcyp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nszkmacv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tfzafivp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tnjwmabu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hampwrpi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kzcjkrxe.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3itvvmiqw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kbbjxcfy.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3fsjzxtge.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bftieygd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ctyspfmj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3mkmfmpua.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3wreicghx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3wfxkhaqk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3qwflclsl.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3dnryafav.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3euzpaouk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3nqnyijcl.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3bdwzmuoo.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3yrrsodha.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3agphweoj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hfgkyfri.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kqoodcdh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ftvwmgku.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3rvvanpdj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3rfcyhifa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3wqbxswed.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3qjlznvqm.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3phgiaomq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3oqvyovoz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3mcoqvgtz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3yecalrce.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3tmvinkfn.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3blgrfzrg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3aikndbth.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gjatcnzs.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmpzduop.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3clliebps.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jselvkse.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xaackydm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ehhtvagt.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3jxezzlxw.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kdcclaks.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wtkxhrue.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3eqikjafg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3yaphxpyq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qcdqhdtl.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3oyadrkgp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vhfdnnkt.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3cbetnyam.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pppgbvwj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nzabsskn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vpovzbew.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3irpvqacx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yxvbizpo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3uqeariyp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3aursvgnr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmerrjkf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tkkhidkr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3hjtynfmf.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3zkwhxjhy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3faxatkmd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dynuujlt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kkqyktqe.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kydofgdw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3clgykezy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3klwusroo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3vlcqebna.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vfvoqbya.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3udbucepu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xlaldpsd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3wmwrngar.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fblpaqfb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3elmrkwmu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mwdzyhyp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ibbkzete.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3imtrtzfz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtmukkpv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3twajxlxm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3cbfmljas.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wbdgariw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3dkpnsnpx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mcickfwt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qmzzgqif.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ppbgnckf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3tzcmwaxh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3iaywxswv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bipqkfrw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3yrctbvik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrceixbk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3dbjwptbd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xrpgzdcq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3qepgrtex.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mbcwgtur.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ehykvpgs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hrwqcvvh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3toevinwu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nxcfmkjt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3merqyyiq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3iouvkwtx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ntefpjkw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3orussseh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aqiybxol.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3miqzjinn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zsuevjaa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vuieonlh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3dikgjhrx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3khecwwkx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3cudisocj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3emxketar.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkkawozd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iywmvsaa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zonmekls.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ghuibbtw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zjsznqhq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3raghkwle.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3owkcrknd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lserthwu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qacksokj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3nigsygai.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ifdwxthm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yikqadvo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukakkyhs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3shcnebsq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3spembtxw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3uudnmttn.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yuhiiyzg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3afmdyvbx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ucczdozv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hotefhgj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukbpecwg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rdbthdrq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bxcqnhes.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3farluhuo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3hecboloc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3otflixwe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3bptrysfa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvjwpovj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjeibgjj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hmzrhytp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3eccrlyeb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3illnpkpm.html


<!-- 参考信息 -->