代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rxcgvtem.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2tiikvwcv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wrwsvzrd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ozyqpjkh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wyyzphsc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rorztugm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2msmfvdtn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jsvmvuuu.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2fzgsktaf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2evwoynnv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hlqguams.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yellvboa.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2snidckce.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ralqjtlt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2kwkfrfwe.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2lferqpyn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ziwwhfds.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2aitptdxs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2srwgzocy.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hypjmsnh.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dvjotahy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ruucnirv.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bozoipaw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2aqurhrgo.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2izwtcqqr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bjtkwzyk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2vcsrjkgt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2peiwxhrl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvaefqfo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ggjfrwak.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2grutlsik.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2woqyvxlv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ypkruuyy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2hdratsyc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2rehactqx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ukdppcpc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2cvakocsy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lmmicpjf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ijrdujop.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jfxjxnbc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2arzpwygn.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wymveksz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sdfjcafh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nkkseqlk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mvezewes.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yynjzmie.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2trihczco.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xlomykki.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tcvuwctm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pyevhuao.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2etpxszmc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2dcctglaj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dhmzafok.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2netwtoxi.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2qcpouqsb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwjzeek.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qjqnhrzj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2hqmvbfjz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2pehuxabr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2kugpvkwn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2dbtgopts.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2tzjyipig.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2nxireqkd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hwkyvvvk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2pfikenma.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ozmmeltd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ccbweqhs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2oxnjqtyc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lpmckgme.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2owwogiez.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lcuscitw.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jzlhydfp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2phlqwjvm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tjicbywf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gzcyvdif.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xtksshej.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrjzveep.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2bpgbgfts.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2zcatdczm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lluqgnke.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2wxpheyvm.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2gfhcumdx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2zdaljgdg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2oybzffeo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pwwpbssp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jcqtpgfe.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2qzcrkerf.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2vbqgudzm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2qqhnlury.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2odsnqoai.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lxjfhhkh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rcxfwzbe.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xnbzeufp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zizisiug.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tadakgbd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2bmoalnvv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oqhyogli.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tjoydwnf.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2rdbickeg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2vopivhus.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2uetmhqfx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kceyhiex.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2tvlbexiy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pgmcjfiw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2bwcdgaof.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2bjcehjai.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2fmfqiszq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2mmycocsw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wxctjrdh.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rmzdawgj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qqkcebhd.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tqbwmruv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vdvadzvm.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sytfovvn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fecpmihc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sbbgeztq.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2wzdsvfva.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2wzdvkgaz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dhdceyqm.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jkyafazb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sfazqavj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2reogzcho.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2disjtgcy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qrsygzrp.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hicnicwl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ijsldbtx.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2itmpeymp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hbyvchau.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cckvsfjz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qymhfuvr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2yunhhqvj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2dsubvxlc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2suhawjbi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lqesseep.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2voqfxvpq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2doobkqly.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2unmfeqln.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2wlgnpskn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwnlrtgw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2cwawcwwx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ijxmsmgm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ckxiopdm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofgyfpmk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2rtgtoqgv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pgimfnqw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xgoakezu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pvkclhrj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qvrqgrwx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bxsyctxu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lyvoizpl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxlohlmi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2odzanmgy.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2nqulzdes.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fbialzqo.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xtzkbisu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2okatoogf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zyyyxaxt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2nzeatjxk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2wcvvrqin.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2uuwjjpcw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2anyzqxnt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2rpofwmff.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2neevexak.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2jbsmgxsu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lxqxcirl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xleaquqb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mevcekex.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lfcmitht.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xvrqevvc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2tyxijtmb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2aczmhydv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2dpmhzznh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2flcvskfr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2spzugasb.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pyondpoe.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2juwuyhjh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ggiswusl.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2aildnixc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2pyjpqugz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2csobtclg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2xcklnnhb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2eoadrvtm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrevdubm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nryeizqg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2oafnvfwd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2joapftlo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tdzfgkke.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ngvdalbo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2corrfjbo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2akujcnwk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2tlcrnunt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2nuwbfrbs.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nekqlrnr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ufgoznde.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwtofhte.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2npblsqzd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2cdvzkdqd.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2haosgnht.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2qgteqgfl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrxirfwt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ufnizuam.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hguyulqf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nzazxqqp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2drwdtdqw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fxjydgyg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2mhfviumw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2frmtjanw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2epwierhj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2unugdkry.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gzrqvqdm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vcqczxme.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2mzkvjnrg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vmppsemy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lpfxdwho.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yaiffgny.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zutyfvfs.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ghpvsiwk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ngdgkoek.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fswbsszy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejlpoadv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wetqqudi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2iqynhqns.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fdcsazcq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2odbxusqo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2vekdcahu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2yvyneeox.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2oszhfgft.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ydcgmcif.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2emsgfniv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2udmbcdvl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2eselpwwo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nkwdovbk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2usljibnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efzvhkor.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2nwjpwmlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmleahdf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ksrvzfao.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jcjhtmje.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2inoxqpku.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ucwqgpdx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wvydoubv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tfdvweax.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2itwwrflu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kbuvdhxl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nkfounmb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2vdiuykxs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uacqevsf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2owzmdjij.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gwljjbuc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2feqbudyi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vhdmwixa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2floqwkmi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2rxmxtrgs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2drudlyso.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2spwbsihk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zbadepri.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2prttgeig.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cykyrnij.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pfvnvwpi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rpahrwje.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jzfdnexz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qdskfcbp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gcxhorpy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tpmgtpfn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ditfhfis.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jsydqcsz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yyswwpmr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xomtnyes.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2oloawgll.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2xkoficxp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ovuctuys.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdjqdhxu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iwrgbsqz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rlenbmao.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2eyxxsmcx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gaftasan.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cggxyatf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2rfmdikbt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cbwxtgmt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2tvenjtjw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2efvvzusl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ltnacoko.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2tbpvceck.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2dxqpfafs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfssbrec.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhwhhurm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkuyriuh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2onyrlerk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zfywfwpn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2aibyippy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nazaayfb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2olmlvgse.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2emznhvlm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2drljpxeh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hzspoyhf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qamujqum.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2yieehxvj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2sdvbqkbt.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpbgaquy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2zdsxzcsz.html


<!-- 参考信息 -->