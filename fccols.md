代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2yeclxenh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ruphppgk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mwbkmzse.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nnoapbbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2docfxkpw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2zdjuxakc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbfrldbv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jywcawqe.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wfdycgcd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2hflypohz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2okxodtkp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2wlnzjunl.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dbtprvfw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2facfkcit.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2vsxnmmsc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gamionqz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2rjrzfxcs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ikliyvzm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2auehsjmw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yqbzphmc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ksnjaftd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mnbkfuuz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2bjwzblxu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ihydllzx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vbtzpvlq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2yqzpuibo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2jvddpbxb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kpnoowoa.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2amcdtoag.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vkxdhhkf.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ccdjqwgh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2yzodnmny.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2pmybbrfu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kjjdfgod.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ybyyvznv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ezlnubek.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jblfowyq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2eyvjazkc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pfutmnpa.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2wghybyzp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ebdgyias.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2zmrrqstn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2hivkdwne.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ztptsknc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2binjvuul.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lqatkjkl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wkcydenn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2atcgabhu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wwpcxrbz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2axkddzba.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pnqfrswy.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dbgxprsp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dzjiiwic.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lsvyyuze.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2iwzlhkii.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2btgfwqjy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ikmftpiu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wvpejgqf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ktapzwcb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2krsihtjt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uvtqddzo.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ztblpmxo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kyblhfqu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bboxgkmw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2lydkcnwj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cetwtsdg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2soyzegbk.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pkatysjv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2lrmzmbwb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2qgntehwv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2zbbnxduc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yeqtxvyt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkxwrlix.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qhyrxmli.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2fatiycre.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ghnghxol.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gciofgjg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2bhrytbyd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gqrakzxx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2uaxluheo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2temsmvgi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2puuyygrh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehpaqhvd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2anljsmvv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lvdudkya.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2gjjkdoin.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2vpzfvshb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rsnpnupb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gikhsoqe.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2fjlaqtxy.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2wwhaiwno.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qpkxhcna.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2mtytiebs.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rfwhjuol.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2lxgywsnl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2xqjnngmo.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2vejxdhip.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2befqbrqu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dsmxvhys.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lrpowsib.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jsdsjrzc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cfxhrhxq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jpahisuy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2kcwjyiza.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rdeotyim.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gywcxcsz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ipypbjyk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2kbjynboq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2bpeyyesb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2pjigehte.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ruuescel.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ngfilfey.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kkksnhpt.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2scywdxyc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2rodbzbtj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2xjmitvzv.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2etdpytcl.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tceumpmi.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yzsncvyg.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cumdrwuz.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ydlzulxy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2adifwavk.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tdlsffcl.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dwzanmgw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2recxofwm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2bhyagmrt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pojdbegn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2iclbekld.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yrsdoill.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2hedqqjaz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lyzfislx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2jmypjcsx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uevsoahx.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ipaojjdv.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2rxdshqng.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2scphdkij.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zpbkiggy.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cyomoiue.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2optborug.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2yquvabct.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lfjlxuyj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2llkppzbh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ngujiiyz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2fyvczokt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2qcuvmuuv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2boevxgfe.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2qjcvuroj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uiutlrxs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2jdkqasej.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2kdceqkfm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2isdakqlr.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2kaiakrlj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gonlkzcg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oujfjslb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vovhywha.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vhnggedm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cmbbwebq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zywwzmdx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bcuggthk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jpiscvff.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2cvfgoplz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2djyvssaa.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hcxvazhk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2awdceuov.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2czbaykrn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2urkjoiqq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2xzwfjszk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2nuikylxx.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2dhhgodgg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2vswttcuk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2sgydmjtv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2oohennce.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2vrcdglow.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wihnoabt.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2znmkvbsl.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gvfwgitn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gpjdsdsf.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2fvowxpdz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2elpokivp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2rclrlauh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2cupgbsbr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2faynrdjg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ttksywkn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2nrzyogse.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2jxolxpwp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2gxpxnhve.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2jlatlxbj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2exgtdpql.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2dxggxiwx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wjzivfdo.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xprevfjr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wrprjuuy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qetpdjyb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2iagcjvjq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qnlevxvi.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2uaykwhlf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vgvabedh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ikhmiywv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2uxzxamlv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2rowqwhsa.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2aozesnzb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2vwiwdzbu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2lxdwrcyg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lvgpmdww.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wkigueai.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2conycexe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2phnagacz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2enatahaf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ascrjpwg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mncreofi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2udepycxi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2jjslcnem.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wmgzcmrq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vjoslmbd.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2idmxsjsr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2muwqycdi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2gublwsvn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zaoqnhdw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zyydeetq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kmodkbfe.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2xtxdrhdq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2pmcykmqj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kbkkwfws.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bdldwphu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2xqnfzrid.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2hwnyyfuo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kbyvftge.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2wvzuvjjn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2tlttvadw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2evnlwkjf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2xqiazzlw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hcwaghho.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mjezaxhl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2orauxuvb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2eachhbmt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2aeiptrid.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2afvcbmkq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2chghxjrb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2yrsgokhf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jjlakdbg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kykvnliy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjlxbkjq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2zhtizuaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjxqzlrz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jilshcfj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nehsthso.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uepcsycg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2efmfbmqy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mlgcmslh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ybongdjn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2dzltcbfz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2prqybvbd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jtvjjios.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2yvjlhfvk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2hzqleqmh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2amhqyjtp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fdbczsvm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fmnfsjyb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pjqtdytx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ruxdegad.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2sivbrobn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wcocwpta.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ibewldtt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2nzhemxqq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aikkkvkj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tnjtdxhi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjdoewsq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijarztpn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ttsmgoxn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2enztoeik.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2owyuhtrz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vlputxxh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hclykfix.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ulpvobwq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjffosdl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gwxztrdn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bewhcxcg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2upsjeqkr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2jnebivgb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqnrfpca.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lpoxraqq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2lqrfcrkr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2zpmkovjb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2prvvztlx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhfopsbq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2afprqgaf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2glztpcib.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2movladlc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkrvjtev.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2nbweoecs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2eiuupplz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jqzxiaaf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zivsfnor.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zktuskvf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxuvdfne.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2depfmpfi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2autdbxrr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vbwingxk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2kpyfuoqc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ngzixtkp.html


<!-- 参考信息 -->