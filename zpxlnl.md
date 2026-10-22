代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qggrqnrs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2mexpurzn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rlterxki.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kfhzedta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztedsdse.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2gxdpapgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgxucaql.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cbmgucij.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qpyspxhe.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2eiynwect.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ajzoxxdo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2rkwkysvf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vfsoadcr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ggvndddm.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2xjoyhqqy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2khgivyoj.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2uscniuhr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ijicotdh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mlxxeldp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2adtmfioq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2demggfmx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2smxlbicn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ehyunisv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2uklerptj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mxodvslp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2eogywbkd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2konthyju.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2imtsutqd.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dryknvmy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vsyegiyx.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2chhwwsoy.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zskrphpj.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cqasadgk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aceqdpdx.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2szokaoby.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2uusolhoi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ruteipbb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2soswzemy.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2mqwtzssw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2uqeopyul.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ehrrkxsx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2egneflei.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2bvvizhyy.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2aausyjxt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zqymordm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2waponcif.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tftmwsyx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pntnlust.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bakgcxec.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2arjibnwn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kqslocoi.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tplpbkkx.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dtywwjqq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jnwmxhrw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2csvrldhj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ungruihd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2csvkqjjh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gowuwzpk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2zuzxmkgj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2tqvugvew.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hkeigsyl.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2seindoyt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lmaaibkb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2yvfghrpm.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2aqypfsbe.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2vrphwkoc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ifiabdne.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2hfzzjyog.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2pgezvugf.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2kfooghbc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ewpjimlq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bfzposoo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ciseknpl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pinexjdq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2evdlkrzi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ayhnlswu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bowhmanc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2gornrdsk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fdvzaoel.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uxjkrhrx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wuugawqj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cnzmqcmo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2goexvhfe.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tbmghgbk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrbnzgge.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2mbacwybb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2yyruudbs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gzgdgmlp.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tzxznspu.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2jzxqasxq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2gydqtbsu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kthjhoxb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xeudgauq.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tapayvga.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2jzwgwdvi.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2oanmarwq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2moxgamcv.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2cemtevlw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2kwyzpczu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vswuvnss.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rcypiwpn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zeyqhnon.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vmurwdwi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ioqxtyqx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fjeqmoby.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cncugfpb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ubxwdscr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2dyujmxrz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2tvvjjeyd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2fjddyadh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2akhpzkiw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2lefcpmlb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yawglmlq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2tjjpodmg.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2rhrjnqey.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2pmwedems.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tqeocnmd.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cdwhyekc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iamyffmb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2prynnibv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fmzneolh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uugsialr.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gossxqrh.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eowjsalq.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ftxajhpj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2eilrehah.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2czzclvww.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ggclfidy.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xuedbkmv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2vkeuanyu.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fdcrioqi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ibvqjxoo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2iujainuv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2paevekah.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tvkaldwu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oryxofeg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qigmcyii.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cxtbdesh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ezsjrohx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2rdirxlmo.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wxfkgbxn.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ozzyornh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2cpsdclhq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ndfabyjf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ybhyvibb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2lkpmbcvv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xoehrizv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2prjenswu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2hylahkyg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2bkrptcqw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrqoqsvn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2jbndnekk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hbofdvvj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vurcfrbo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hxhcvpdj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2htstmxch.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zthhsjem.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yhemuyri.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ayegazuw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ugnvbbyk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2tiijbolv.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gigrekdk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gnugtbbd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2loyifrtd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qodwfwpc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ukspzoxa.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2izxqgsqa.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2dzsxoygi.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2imtvvowe.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2tptnfplx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gzdqbavv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2wevicwtq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2uksjkkoe.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2amvsxuor.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2zqikmmkf.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ktzmirdh.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ebzjsbwe.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2yiemzktt.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2kvnnfozd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2nqzbpzjr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2uzmwaguf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2igurlfaf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gfnzmfbr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2nahhgmyc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2tyzuwqcq.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2mxbpcqls.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2rrxmkivf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2tudiexyw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2grqmxqrt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2seybefta.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hvqualhd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2juqxguzf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ursbjcuu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bphfwzzc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2immqtyfr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2mggxopqm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kfvyagdf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2amgsmgxc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2mhcdqcpf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2jnnqzhxc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wnftpmhn.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ashqeurd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rdidkczu.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lifqnhap.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wosqixgo.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fcfhczuo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2dcjstdbd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2llzzpapv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lybiqxvs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2sjprsyzw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vpubefva.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2mhwcyxey.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2djxmhpjb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2xyiqkcje.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2hdakybnr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2uyelwarb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwjapyix.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2teiogkuv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rqmstwla.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2kbvtnzvv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xdwqjfbr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2tkmqfcgm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zbacrxuo.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fzyvhjmz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2cdlcwsnl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjfxhspm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rlkmqark.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dilusqxf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2cdhhdphk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ohntxjum.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2jgrynmwb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jluctcnl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2yodlwejh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2rqwwvrpu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2rmpiltpv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2lmryuvwt.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2suhvtoxk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ltverata.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2pajxsvtf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2vocxtbev.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2snzjmgng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xljfxzlh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2gangughx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqyzgtcg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2dgdpedwd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ykurwmqx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2rkamlvir.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yztzvxcj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dffmnojp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jmnmwofw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2tqpjswdb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fowgpfwf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vhoczysc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2rrvwiovb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2uaogucnd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evaoafet.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bfriusmz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lisrhzqk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2obmswloi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2bfqltpja.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2vuwazlmr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ylehiwmw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2aromjjte.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cjyozgbl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nyidljsj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kqbniywg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdjltwwd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fplpjuwz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cratpgqs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cthdykdx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mwnvnrsn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2czqryrzj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zqjgcyzu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2tpglblye.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2sjnnqygk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tynserrx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqalfvgj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2pagcoczk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2hsrvwovg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2rxtvtalg.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tyrumczg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2cpdsbylh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocjfueqe.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ooiqwefo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjcsugkl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2scmqfksd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2uyrxwjtr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2unmnedvt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkdcweno.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2btegknlr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2nlsfurkx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgtbrlqu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2usmyzjpv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2punfeatj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2fqokgcnp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pkeypfsa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2remqmyfc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2afarxwik.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xjsducaj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2rsunqpzv.html


<!-- 参考信息 -->