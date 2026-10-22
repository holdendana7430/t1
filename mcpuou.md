代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ynlkvspg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hcndgeco.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2hamkexxw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2emxqpzri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqynuegv.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2morfrmjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygkzdrfn.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hehrbgmr.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kjpreowm.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2pgpbigro.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tjasetet.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2waarvwye.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cxjtvczs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2bgwvsbsp.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2gddnklit.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2isagpybf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2hblsmcdh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2kbvusfee.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kxqpbuvb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ztencmsm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2vmfrulrg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ewlhpezr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2txtofumr.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2japsenaq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mfmnwcjc.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2fwfygijl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2wavubnmv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cgybdtxa.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wzggtopq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nphfxbhb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kfxtdntb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2xrfnzsvg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zufjhfjb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gsqnzrlj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fwwrzofx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ecemtcfk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nipttjjb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2luzlvxks.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2aixxnmfn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2nuygyzxg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2cbilurww.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2halvwdei.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2jysfdnkn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2barldshp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2aegssosf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yiqxifpf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2blpsxyko.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fohtrrzd.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xgrytttm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yljzjfci.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fwjzwioh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uuinesgb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2azlotnch.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zegjzfap.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2rvoijwcw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lzvxxuej.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2aynsefpm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zhbncrdf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2mqoxujbl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2frcepbyf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dkezdlux.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2jnxjzdde.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2kjpvljqj.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ylxkqlpi.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2kcgctihq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2mknybqfn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2abbtdhqb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vtmhyxza.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2jvnhbyxd.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2kvxyrltr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2xdgtqsqe.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ghupupsz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbnlezvn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gldpvdto.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2wzubmerq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hdjzvmuc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sdloeeyy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2myqvmfbn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gummsird.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2webrjtyg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dpmupgzg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ofankwae.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ucftfwua.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fccdnsos.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nrqoalhd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2sloluoyv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2zsoreffd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mrkpxecf.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2frvdzodd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2tbmiezxy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2bdxijoee.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fiygzsfl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2eyidtosf.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2igqesxrj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2czffnnvj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2rwtfvjik.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2bdlinoed.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ttecngzn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2wqlpllwh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ptdflcyh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gvtnkclu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yemozgeb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yjooadth.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2towufcrp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fsubauot.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lqpxaiui.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ncmmyeyq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2hlcqlhkv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2rydefynd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zrvspyrc.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2mysytdnf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dctuyupf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2olzqomus.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2tubuldbb.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2umeanqtz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ppqoponr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fixaomgv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ugnittdk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2keybnqfb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jaerlfga.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2teghuwzj.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fattqbvd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hzpjoexo.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lnkzwnvi.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2afzdjxoe.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2dgwzyerb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zsuofzga.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wzdumxfy.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uelgjamb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2hoaosgfw.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lxbanwya.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2adqmfwaj.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2klkvpvus.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2kgkmrucr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2bzgkgbzp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2leunbpah.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ldhowmhl.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2noztsxrx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2dzfmojlt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2zzyxxlqh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lznppgql.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ekbiilyr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2rlyfxhzv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2yvbaxrtx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2pdilgdvr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2tyaejxmd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvzoaqwg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2herbfodv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2oeulbaal.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2luqywexr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hpuxpznc.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2bmiwnvpc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xchutuoc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ylrdhisy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bmxeyjjy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qoqvtpku.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fjyhltlg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rmohxwmm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qqcaxphc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lxkacscq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2vvcrksoc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2fhkefjsg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zbcmqmhh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pnjxibus.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vconqkrm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2kjngryfy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2pbuyynyk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2yxoixsvv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2yqdpllxh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2olytjfpl.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vsrfoamp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2jdmpeuqk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2sfrigimr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2iyoaavjq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2syotolhj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zjncbbay.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2prstnhee.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2mwmqlfhd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2dhgrhdtv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2wruwsznu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2zzmojdpw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2vtlisqgx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2smsmmdew.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2knkllxog.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2tinposje.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2zbkgzgff.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2fxgtqaak.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2vluvckhk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2wnxyttug.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2oopgfsdb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cgwegcmg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qjjbchlf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sdudfbxi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lmldjmba.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zxitloij.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2kmaqwnra.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2eznnouae.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cpzozsme.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2nofwzixm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2hvrsssap.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hngotuvq.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tetceaab.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fyqrvwsr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yqoaktgh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2nkuijeae.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ialwjrmi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2snpuxgci.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2oqczwihj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xymzhsar.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kwzmzmhc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gxuhrjyh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chagmrac.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2szaehtex.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2swgwvbfl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2kfrhdzkd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2espywrxl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hkguyenj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ihedmcab.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vhdvcebi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2nxzvbzix.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uojdcgku.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lphbracg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ztngpjqp.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xocoeoss.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2amlcmavx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jortjyds.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxuhwoyd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tfdszuwx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxllfhfy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2crmxrtsl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2wmrhkcyy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xbeuruup.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2vhtabisc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2pzvucvfq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2gnamipzf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ugvzrnvi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2zarwehui.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hevyozou.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2vjyclufp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yegyzege.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2fltumryo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trclqyde.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2bkqghwbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbifiarn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2nofgbwtv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jnfsufex.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2smdhqodx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ypwtykpq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lhjuhmcv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vjekgqnh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2elbgzyit.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2touehgrw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zxfbdcns.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2tlaiqxyr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2oicjslut.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2myveftgx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qsdkdgeu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ebfaxmdy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ogrekshp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ivrdbjrp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xflswgzx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2znodhekp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2lycxzuoi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2kbhaaiha.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2culsgeqp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2btjfrrod.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yflycthg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2htwgnsjv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2eywlqedb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ebbuulhq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bqtuhxnw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tcehpoer.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wafgrgmf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2fcwxcooi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2znxxvqkt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdapthgb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsteppby.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vgyvznga.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2akkwnvcu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovjlrxom.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2khajyvoe.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2nlbrtnxt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrbcqzvx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaajxdkd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aixoggxr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2exkpaaep.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xqmnckna.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qmcexcfj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vprkzaur.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ilsxntud.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2dcbvlouo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2otlufqgu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfstyska.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qffjqtsi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gmmawwcr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2acofnueu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nihdoorb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2nfzmynie.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hklfhtkg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2goydswrt.html


<!-- 参考信息 -->