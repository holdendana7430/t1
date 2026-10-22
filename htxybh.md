代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wshqojom.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2vwljiwzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tghffdhj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2crbeexgu.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2jkdornie.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2tciykgtp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2btatkrkc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ziicnlbh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ypbbtngc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vhiwkwzn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2sjcrrwbu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fyyfubkm.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2xomgrohq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2pyudkcth.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fuxybnja.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sqzvtvrj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2vmtldsgh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uerjwelj.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2hjzqvjqj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2hngilckb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rwylzzzt.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2wbjlbedw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2epygbvyr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dacyunbg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qypueyzx.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ondjwdpq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sffsgnno.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mfxdugwo.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zuzniajb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hurusmzb.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dklflzzp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2cfpbpcpn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mwxmwruw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2bosugxbv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ztrimeuw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2eiusejvm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2lnhneynd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2zdudbozb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2vumqglbt.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2aflnmtzw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2afdjniwa.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sboedueg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pgcbxebx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mrqirbqy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pazxmwzj.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gafkchgi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fjpaubjg.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zyewkhlr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hnvbhnul.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vfswtach.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2riuarxlk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tbyxgogk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zpqwmrad.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2eqspcydg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2nmdakvkm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2slvwsknp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qxfxzkuh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2xmkpkovp.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nepqkydl.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xcbwbumq.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tvhptoci.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2xolqtsnb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vfmejksy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rkzqhpao.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2qfzmscvn.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gubjpmme.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2vtvlmcrr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rvjhcyor.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2fdiupvly.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jnzdgvdx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ouwxrhei.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sxtkfmpu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2shyckpuv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2sgytekae.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bgafkfet.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ndgbnfld.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pebprnjv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hzruchwd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tmleyhao.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pvnatsje.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rtaiicnc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2epquyvrc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ubouefqr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvxpnyck.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2hbzbqvrp.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2qmlpbpil.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2latjalah.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jkkjnxlx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ownwrzrj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wktiatbp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2hrjlylvv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2napastee.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2evfwyifa.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2jwzfgqey.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2fblergbs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kjmgyxfl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ynypawuo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ujjvoxvf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zvjmznyl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2bcugbdst.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bszagnom.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qzsyxalh.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dwawpkhp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2smbrukjx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2utfytutq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ytmdigyu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rklxqniw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lczooqyq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2lpkcfipl.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2krqyhbqt.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hoeagbsf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2dyeccyvd.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hzxccrmq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gspwlvfs.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2shziuayz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vqcjpnwn.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wkypgffa.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lhqjsepb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lthdzryt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fykvcutc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ggnaczyi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2vmvixflq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kxfjirpx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bwmxmlje.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uqxbvmps.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2xoqvmhfc.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xbefktbv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2sjhobolh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yxlxqiip.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2uvcwsagm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vhsqxfmb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eidzjnxy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jznjwszf.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fiosafxl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2totpsxev.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2rmehtqbd.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pfpgggmj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2atljsavo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2vbwpkplb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2jubqjsiu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ioxhkpbd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2oqnanwzf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyckmroy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qichschj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ekkfkymc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kqpkmkbj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ukvjtuwq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2wwbmhcsg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ongegckj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gniybonf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wpdfzdwb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yfgzljrd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zjktrwlw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cgvhtqrg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mffhqbvy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqcnhelt.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2dyfypiks.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2knimadjg.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2diuhywmm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dypslrqh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jcwxorqn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2omfynskr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2mijkuqiu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2vcbfuczg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2xtselvzo.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2iedcxmsm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2svfkemks.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ftbkbtij.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wntzfbhe.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2kmpqadls.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2misvdijf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2iqgnkqqr.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dnjnvlxk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2pjqlatxo.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2dwqmjqwa.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2nlyosakq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2gpetcshk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2frwscxlj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2neuyxart.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2pvejyqpu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2cjfvhpis.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2lirtzyqo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2lajxhyea.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2wblzbbkz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2rorfbxkz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2djlvosau.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2oaecqoah.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2werojpcm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ymuluyuk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pdrffkzs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2okmzhwxs.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2diuwhjbq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2asjrqwgo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qwkewgla.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2vomdgdnq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ohblhbcu.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dnxfnfbb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jujhiznv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2iawcooia.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ztpqsmdc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2yttgdmga.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xsmkgrox.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vkjthzno.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2yuyuhmas.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vhwlizow.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pvrymyoo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zdmnjvea.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vdkkqqai.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ewvnhzzs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2bswprhtb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2zhlfdmwp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xlnsqqsu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2gpukdfcs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tfhwzqfb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rgubrtuc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ebizeyxi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2putzdgqj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2yfsizogv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2aucmuqcl.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kntyyart.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2wfdalmuq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgmnszco.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2embeurvj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jwalycsr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2vmrudhqs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cshbhjqn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2titnqzkw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xfgtcejl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2wqrhjcso.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2qqxutmsl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2kxnbfxvf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2zeglibto.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2gdhnzjqg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2pdhmdtfl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2qfhgumxl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2cjcrbtgr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2yuevgohy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okancbjc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qgnygydx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tlurhwza.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ialiobrg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2swbzxnnp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ftvzjtiu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sfqhrpak.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wpgqynbj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vzryqiwh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2pzmiizor.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2bzhxcddo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2htsoqnti.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2myhdgajb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2lqjrkyod.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2jjshciqv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qilwcouw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fxxdwlxf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tksyxlzh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2mekzqczk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2gkuggepi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2teeufjrr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2snpqswzl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2mfgwurxh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ayymfwxb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rjqoqpog.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwlxyazh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yhivucju.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nkcccvmv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jxiylnut.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ptktgxly.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rljvpkpe.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dnlzxwqn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnjvtzdh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pyjzhjoh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfazoctq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybqszemn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2jiuaglab.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kcllvwqp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2djaetkkj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hloagbtv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2dbeshkao.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dbjizycm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2esovxsbd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcktcbgz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwczkrzp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2fnjkchre.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ajxgmsdo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsddiuwf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2arepcvup.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ohoiljzr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocmilfcp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mdgibnfu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fotdlufu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2aewqdotb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2qcrknbux.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2synwbiie.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2tyczmiqy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2msenenoy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qmwlfypm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcmzjoxu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jbmqwviy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqcsknbh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lmugqucw.html


<!-- 参考信息 -->