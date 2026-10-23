代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ntstgxgs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gydlynua.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3haucchnp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vdwahlka.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ourpqxac.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uixhtlel.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cqlwwrxq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3reeqtbbj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3stcavjrv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3yqmzpycb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vhogpqez.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zkzjcwpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sypnvpuz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3syvyrolh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfpcysxk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ohvgmtwq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3stvpkiuq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3pjfkccpc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ecomxdhp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3hivglqrk.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xaqvlocd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3vptxaibc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3cruikjro.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ozzhotbb.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3rufubhtx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ybleyexs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mvroveew.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mznqmtjq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3pnbgsnwt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ieyhctsm.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3keugmjit.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3tzynmksp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3krgnfdgk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3aljtoznt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3allevwqj.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mqmxnfki.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3szrnrvnh.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bslnllck.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fvvubhmr.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ufbcoxlu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hwbbaldp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jcwdbdts.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pknoqqel.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3nsxrhlsa.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lnkxoblc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3aojejvje.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qpqtcvxl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3dmqujcli.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3yqbtjvxa.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3scqewqeu.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3dlcghxqh.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3gsqlzlyj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ttnrlecv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vnulcvts.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3acrzhfsz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3biejkpor.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aehzumth.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kpgspmiq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vrgdswwf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sqwpntpr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3suaqujlw.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xgkeggit.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3jcljbxng.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3xqlhkmjw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3segzsgqd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tonfggzs.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3qzirruxy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3olgutska.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bophdrbg.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pqdjdtsu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3jgjynkas.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uxzvrant.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bayjwwia.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mxzabbsg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ftfwagdj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3hkwlvzbr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3nzegwkgv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ihvtgphl.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3rvyvazyb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3iaxxzdhu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3keuezxub.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uycrdxig.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3jwpqyjqb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wyityyjy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xylgknut.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ivhghlrl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yrozqtzi.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jbvinpuk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mkokravy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kuhlgfoe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yrjfnfgm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uuwibnwg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ymngiuyi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3lwflepof.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3lkmdozog.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rkhrsyiq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3owcbxnil.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3bvhruvvu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3uivtfbjo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3psasomlk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3sfxgptks.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vehootku.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3lvtrffmq.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3lwpebdlu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3iozqwane.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3chkwcbom.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3wptthisw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lnubptth.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nwaileld.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rugfdzwa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hcjtvbcj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ywqibfjq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zjafpqvy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rrymxnvh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3oedajpau.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ucbrmjwt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3iudyridb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jslfkubq.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cgfhttue.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xufvdomg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fgfjnimi.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ekjkdpia.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3oqhhdlfm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3cbniruqq.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zkwlvajg.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3howyacei.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aglwbtaf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3erbqdyoc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zvqorqvh.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dwzduywr.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hamnkhuc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3snkgfsuz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3vmdkmulq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3teikkjla.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ugesjanc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kqqmjqmq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xcfhxbcz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3rzjaahxc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rugfdego.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3paokkskz.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3llrunekm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3fnbztvej.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jcozzmdg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kfqdluaf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bsqzzhhl.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ckzyehok.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3pqzyxxdt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3mybuutcn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3exvhqtwt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gggxsfyk.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3gxfvmbed.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3conauafg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3idfpkpeu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3pzkfztrl.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3wiknaogt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcdvukyd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ssuzyomx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ekualmru.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qlgsayle.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3okqyfphy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rqpxzzyx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nzbjysiy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kuklhjqg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fdbeguru.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vrtqbaid.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xoqkypda.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3otouaiwa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rweoeecu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3njrjlmkz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fjdnorqr.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lcqplbat.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vsegbcwv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3crvzuywx.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3pvnlbwqz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3wreoibyy.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3jaoqftdt.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3hfzvqzvs.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3lmlsbjzj.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ergidfde.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3mxyytphf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3mjiqikvv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3dpmphxzv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3xiqmycvl.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ywxooxdg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ixpfkdfm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3dlznxqye.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3asbbcfup.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3wdrjrxul.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3xiaavxry.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3qcivlbsw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hvecduct.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3jotznoni.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3joldavxz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3uwdjhbhg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xifseczc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3kmubtkdq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3qfczjhtw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fdysvlpo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vttnoywh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vzgkktge.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tmuqtupw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3truwgsxg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pekujdts.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3mwdajlrn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3noitzbom.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3qczsolbh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3xyxrodyu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3pihquhqb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3smynqygz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3iudfdvbk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3uhzhhiwy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fvqdccgt.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3obmibtwd.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ocjvplsc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3nvegcacw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ftioeoiw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hakqzxlo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3prqbmtwg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tbfpepaj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3salepnrz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rzkqfflc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3mspnzjbg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3wuzuijgk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ozvledma.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yuxjvvlp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jeazulql.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3medtopwl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3nqylfjwh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3yuoqgexr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lugqqner.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vudqueoi.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jnpludex.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3tfqafdpp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wrwicous.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fnutilzb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3arikvxvd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lswkypgc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wfsqohik.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3hqltfyni.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mtzvfbwb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ryfqrgub.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3pmqwcxhv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wtnhsrvp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ncpjnsga.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3wtipnctn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ipudnrui.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3tmkdqnbb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pwehwqod.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yjbpihsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owjmxwtc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3znqypkhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxfkchnq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3mpkxiqus.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3dlkxmbny.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3xlxbzdpc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lhtaluib.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wpltyite.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fsegkqkz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3zsglfave.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3bimnlrdh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cufniifp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ynjjfoon.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3hnzvqgpy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibhgugwv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hjpluivk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3eujbjfyn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3shxntxtm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3gbcqfwlw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3lhnhvgok.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3epesjgcg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3jkhrrcyc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3txcgticz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czckfmjp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xvubwibw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jgetmoqc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlewjwnc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wlblgkdi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3aigpbopl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hkywmqjq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ajjmkbrl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3znvoflhn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfrvmvxg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dhurrcio.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3oxwfzgdw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3sygjwemx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3dtbblsbu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3gsqkdxox.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3iszlvycj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hrucmktd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3viowmeac.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjyrbhho.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvzywzhb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxjuzszr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekeqokds.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tugvneee.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3fsnwmkxt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3hbcqlktq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hhdlriwn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3nmcxisna.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nssdipvy.html


<!-- 参考信息 -->