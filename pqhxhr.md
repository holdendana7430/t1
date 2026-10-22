代发 wailian999

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vahayqie.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2aoweyxtd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vixvutxb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2unfypfpv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2rkfgvwzl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2oqislrew.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2hwuqyvfx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2yjmdxhod.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2tpcxemwg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ytvhmssc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ozvizunr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rhmpjfnv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sswzvsqa.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kiolnfuf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2texukxll.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2beuvcghe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gcwmqqhe.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2odnroizf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2cqnxjrcr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yftguwwc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fmkrsbcb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dnnpljft.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2snwlikrh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sajpblbh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2gmhucixv.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2phaaavzw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2enqhptqm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2nbkztkhk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2vccxjzvx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2njzaxxpw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2yyzzodvz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2lfqjazdk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2njcpfbgz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ehlzkmvl.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2veqzbzsv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2azfjysiz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2pjorddot.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hmrdhvri.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ibfsjbns.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zyjpuyhn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qayxurig.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dwhqzwdx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fosgyxeo.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ybriikdb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tcjywwbz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jhpelemp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2wgqeugkn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tzmakast.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2viifquwn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dsnadlju.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2znoarzdw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2waxqeymg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2oimutrul.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vecdhdfw.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2legfvjrb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2tgxpjtvt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2hsbnrqbo.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2uzfqhtir.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tahgxmbu.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2agsyjhiq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2jgrhswai.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qxgloaec.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2vsnghhjv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nzfcmpec.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2dmichcsf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wxqzdnob.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2frekytjp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2canhwqmb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xpvbruhs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2rekolppk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yksuczov.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ehpaojkv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eabtrjfx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pkjvbhnn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zzxvdsyo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2unjymdox.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kipvooyv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2xrsmmnuw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2trlrircl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cbgntjmw.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2fzezqjrr.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2hknainml.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2kyixdltu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2amelmbph.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mgqamkow.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xvkyqxgi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2tsdiwbym.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2jflphkkm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2dmmaodee.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2dkcopqks.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2oqpenbkb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xkjzfblh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zwpdwbqk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jzqvksdz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yczerxct.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ieidlbez.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rsyvtkpm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vihwjtsh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2chtqdfqg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2hpqqsuis.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2hrzghyzf.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2yttehwww.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2yfnaheya.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2uvfqrksj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2snpdwkpk.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ijxygpvg.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wgzrbvcz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2lbwlofha.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rbcnayul.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xqemchlx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2msmxuoxt.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2clngljce.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vsdobova.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ypjamfqd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gxbsbmup.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yzwbcjun.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2btbodggs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2jgwktajr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jxygcjgt.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jmuhibfb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qhxvzadm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2eyapneyy.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vrgwukot.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2uzyhwtqq.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2frccisjz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2pccfimfv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wpbntkas.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qklqllsp.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lceosdhx.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mvbuxvtu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2lrliwqck.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2bwhfzqes.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2faakhazu.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ugksthtu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2acpeybay.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2xjglnmim.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2fdsxpreh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xepegrqk.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ohmdvbsr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcapyxgw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2chlbrouk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2isldcxav.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cbfrsdqt.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2urjngkpa.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ksjioilg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2scpatmur.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nzeyawun.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rljtdife.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zqyzorwm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ayjwucxy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hzhehbye.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wamurzzg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2rhrkubcz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2itofbeff.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wfsuiywe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dddwhqiv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2sbfkmzee.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2nfukbrjr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2bcaxnlpg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2najrviqb.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2wsaxpfvi.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2kprzzfkd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qaiynerv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2uhynhraq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tvjwvdkk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2iubegdrw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2klnbccmf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qrojiqfy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jylypghn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2vyreqmjl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jvvcnvmh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2gritjstq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2tsivugvq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qwwvdxnn.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2vzzjctmz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2stvxsisb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ubflbjpj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2mnfzokpc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ewhgtvfr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ojokpeuk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2anfghjls.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ctxfjgcs.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kkdeikbr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zdnubguo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2diujqkag.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2iwdezrwx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lgyjihwx.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2gnoeywqu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wqjgsnby.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2kmgnedyq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qggwawiw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2jfcfqqae.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jdmzlboi.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jpseaggv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cceddckm.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gnjlnrfc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2dwevdiru.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gecehdcr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mktdcujs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2nnhyjpyq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xwobrtmw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kbodeqqj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zgouhdvm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2isiuampp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2iicamdqo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ylygidvv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2iislurbc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2msxhufly.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2mdznxzhs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vlogptop.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2sbkbecbs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2xicpvkmj.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2zgszguoq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2kguuccpq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mgswqsrb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xahgsarn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2fojhxxkw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozysxlqz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hbdxkmwk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uyamkori.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xadmomqf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hainajiz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2myjgyblt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rpplegnh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2imzlsaja.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2zffuxfxi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ikjcpiyk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2lzcwzuqv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2obrvlvnn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fxhkmmyg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2honkwmgj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2cnedsrhi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jeyjooso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybfwonyn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2swrtmeyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyfhryur.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2zwxcdoif.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fabbxfuf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2wnszians.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kcvbvths.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2psayesql.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2csrkscsd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ekmiseyp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mbrwzxrj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zwetjmmi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2zinxoxop.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2dcvznfih.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2giehcmhf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rbugfstk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bksgxnqd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cbelprze.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2uhmezdio.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2voyrkdya.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ybcauhur.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2aluszgpz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2yjfjykeb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjujwnal.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2matzuahz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2clugieum.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjreeqcd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nlgvadgi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2mcqrxuqx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ofsutsft.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jfmjpowv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ajbrxttu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2mwnbrzas.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzwwupxc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dddtbdhe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ydxlittj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2zchqcwnz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ovwfbzft.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2rfsnpbib.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kaayjglm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xbcvdqer.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2blrpnrzy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqgmbvsx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2czhgotvj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rljusuhd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2whnytdjp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2vdiirbcg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2doymepcm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ixwjznpk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jujfrkqp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqyvhflj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsufcddp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qleunqxk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kktdfwut.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gxkhfbib.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hmkdwqol.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2hyiapgwf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2tksxpesv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2jvewjxne.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2nulruoss.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mreijzuz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2csqfhmra.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcquhmaz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ynvdhvqv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2mqiulzak.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2notzzooh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nzumdgab.html


<!-- 参考信息 -->