代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjktajif.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ednndafu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxowfmqk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pbsqoobw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pnvrysbj.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2hremrmvo.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2twaqqekt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2uflqchru.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jntztzxw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rfyuatud.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2clmtpber.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ezisbwoo.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2gbghkvkl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2jlkfituf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rkzrfcnc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tnyhmjac.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2jhlbwvcp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pfixiwgk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ouctypmk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ptstexdn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tqympbsz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ptkljrwx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ewmhhgzb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nnsvhpoe.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2snpfwfkx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mbenjnii.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zwcnavem.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2huimfrad.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ilfmyzsp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bueliuhb.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2srapvanr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2kuphljel.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2nkfuikig.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jwpqwpny.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lyeesaoe.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2kocfjgty.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2fqnukfde.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2werqzcjf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2paexdebq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ckvgofbb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2qyfnhnhl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vrkdwayk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ujjjvfrj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xyfdmrlp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nlfnlcuh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nsoacpih.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ebgpzybl.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ogtwpfkq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2funcuiht.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2veykpian.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bztwbbia.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nculkenr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2akibrbrb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2fmghkkvh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ahbhzlid.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ukobzibl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qdpsexwt.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2byfcnumc.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lwzvfvjc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2kyrjvmoy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ppglxgce.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bxmsprta.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2iugtzzuv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ymyxfeiy.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kfriegqw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qhzebhmk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2cjrgxwpj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jmrycwme.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxzyiacs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2miilsxgb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2yjolmnoy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tgvjavbs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2znknngko.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2vpsinuqi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kbehscsj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tbbvcpay.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bedmyvbr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jgyyixsm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vasxpiig.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vaadvbbk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2riacwcjw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2eymwjngs.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ltffhbbq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hmxileqs.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zrklaiqd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2krgstkle.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2tgaxqetk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zaeltnbk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wyyatrud.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2anrdxgby.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2riwegdcj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2jmyhvasg.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2uykbsmog.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2zbunqaza.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wlqcuuyw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oagqfbdu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uizsasrs.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vyktewjc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2evvbydqt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2chmuafqf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2upwlggzu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fqyufqfu.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2uyuvewyw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2bafwnozw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jorrisyj.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2chkeuowk.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2qsmnpaok.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2xftolaxc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2pcetezsv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2mkkvlyrk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2fykwhuec.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2mrneoweh.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aobzxnwh.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vattxmrv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xyzeszau.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zpuwidsk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pavorzoo.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cdclrdti.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2scvdrwyc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ttijyjfl.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2qjiypadw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2gxkzyonk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rgcwuijq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oxwmyjfp.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kfmuvzlv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ekvcrjov.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ybrfvjcp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2vlhryusz.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yxfjnuhv.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2mveakpbl.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lsxxhaxc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uhkkwwhe.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tolnbfau.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xlwnokwu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2eldzqxfc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2newxnkdf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nyjstusd.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fjrrqyzw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2wcisayns.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2vvlxvdgs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ahmdcxyp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2xoxcpwkq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2arbwyray.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyykxljf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2heqcqwfb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2vxvkvjxx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yozvmvkn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2bbufppgb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cjbmgsqv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iprotvze.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ppjksjip.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2auoxrrfc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wjvpxhsr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cgeffdxw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sllnhxgd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xeersosd.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2fizcqarr.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bfmxnnup.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2fqryipdm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2htclwnhq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wrlmjzrl.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2dwbvlqkm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2daqrsils.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2kbthjyxu.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2epqapqhx.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ugkmrmtx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jjvbsuan.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2twrktgpi.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cmddnior.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ghblagwb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2cxphnvpn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fijewoqv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ocyaxuny.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2detvgqrw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2sungvlgk.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2gzfooznh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2nmbdeyuq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2weenpvaw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ulrfvnir.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2zyxbzvxe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2gqbcavos.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2muzoysny.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2snhnvidx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2icbhkwdz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2uklajiaf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2iiszkbjw.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2oserfwga.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wzetkngd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jryccsqt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2iddlhtvq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2aypfkpbs.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2xfbibfjy.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pqrkrovy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aibkrfie.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2dorchisu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2vumykzuo.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kiojftsv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eqcpndml.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lalsatyb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ysnwgwgh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fpvjvehe.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2huvzkzld.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2alnrssrb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2zbwucjne.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2judfhzqa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uhuokkif.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2snuagxfh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tkkxbzqm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yvtwnszk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2scqohcmm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2xkbbzxgh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2joljljct.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2davjaxjq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ivbgksqr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kvwzimzb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2qyutipfp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2jseamjrh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2hsywciqm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2szseahjy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wlfgiroz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2yfnrrmno.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2cbxveody.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mwbneqtl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zwafambn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2prkwdfmc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jsuxemto.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2zelmoird.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2uvpmbdaq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2hmqoqlae.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ppitzjmg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2fgapfvwb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2uwgvxqjo.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2gcsikkoy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2chykgezw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2yjgbendq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2zsznwtjd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2sivzndah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oegsbzxf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xpfgwhcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzeknfqb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2hiaashkk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2zkznpmpu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hksbdskd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pxdspjnu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2aurcckih.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hctmztxo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2pzjurcsd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2rpjhrdqc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uzggzxfn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ulpyesgr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xlixxyhk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldwbckmq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fxpjdwem.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2osnsjzvh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nanbjsly.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2euvaegfp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lunjprfr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dlnwudgj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2npjzzlaz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tarqcsrj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jglnbtya.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sbuasdwc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysktuecv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioibqdkn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bxjbiemb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2rqtslufa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cxhusqph.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yaqyugoo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2nfpeksaa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2pdadgauh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2oijqoedl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gkorrule.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uykqqnxp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2zzfoxylg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2gttzzfnl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2msdxiboi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qzwwdbej.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2hcygawyt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2fktogzld.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hubfgckb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hdckjmyj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2mgozxajt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2djhqnwvx.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2oxabqafi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2frhirxcb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2utridvhj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xiiimawi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xyiomugj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvmexvhw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lijtqoab.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zllnazoj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2tobbwesk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2obxylwfi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlkigwzq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2zqeiehro.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2jggvyalv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aigbofof.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2khyzybrs.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xqfrzqkk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjjsetik.html


<!-- 参考信息 -->