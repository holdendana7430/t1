代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dppsalbp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2efzrudui.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2xfcbbwmm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2updbhqlv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ycumtrnz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ypicxoij.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2vmddrxqd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kpamdkto.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wphmpbyj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dodvxfic.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ktwxnurz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wqpkhdsh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sgaaktff.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kduglqhj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kcjezaoj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2cpfcjwpy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dutruzaq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2okohrddo.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2oizvypng.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2fkmscrpi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2hunyreda.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2tgbxvsvf.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2cijpnkcp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2zcsdpheb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zidcghcm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wpptzvjo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jhblldtp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2btckvahb.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ktnpmijr.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2somrwrkw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2llrvmlse.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hqkukach.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nwpzqjlm.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2oxauclmp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2kyliimvq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2shzhvpqv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2tfdlvecc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zgxcgxei.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2gdaapmvy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2caprzxih.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kvpqfxly.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iadlgfky.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2epnakuul.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bknlyxan.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2fiffnisu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vgwgjmfb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2aersfmmc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2wiplziio.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2pyrpbjcc.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2blphbzah.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2dklzuaqd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nzxylaps.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ljmroktb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kxmyczoj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2uadvbecp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2csdytdfj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cstkznex.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2vwjfumoa.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2exanxmjt.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lhmtcalw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rdljyjdy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2daunbvyy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pxlhtsyg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oznyynsb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cxbyfedu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2mpfvwmwk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2zygmarwx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ezivmktt.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2laipjstu.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2fqwcbmac.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2arnfsbcw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sqziygsr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ylfyctwo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2pfzshfgf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2xfklezfb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2fsaqfhho.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ykkrfrcw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2zdibqaya.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2euosklqi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uvsfxovq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wilhwekn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dulkcqmb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zijxvyoa.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2dwxpomvb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xmgstpxa.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qpqlclac.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2xfugkmly.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2mwbprewc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2zpjcotef.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fmijvpiu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2gkinpsye.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2azngsnvq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2wnbkexxr.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2kyicmuub.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2kajghglz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2cwlolqaw.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vrivfjdk.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cbbpskwv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vgpcysvw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nbfnowzp.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vrkldskz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kthcubrr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2avvophrf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vlzdcyav.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2acxbjnwa.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2cuffiqpn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ziwrhyhd.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lltejjxy.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yoqbmdmu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2rsmlnmdq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2egurptzj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2yrrvupdy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jgndpgmm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2rxhpbdmg.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2eynbtwzk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ytfewvhk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mhneiiek.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mdxuidtv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2lffhlftt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2hlxtcxpy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2awljudpj.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tdfexutp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2zzoxudqk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vjbumjjm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2bwvuczec.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2biprzjbc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hoyzrtsh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywabspwh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rzbpctdp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ltmiztjz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izesddwt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2nwbrhdku.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qfuhzqcb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wyqzbbnp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bzhhkpic.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2otknjezb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qetgpmeu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2agmhlhmq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtvxethm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mhrliwjv.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2yntawlal.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qjyligsf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hoibfvmt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2uagiwtoh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2pofbsndk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2vbvuyarf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2gzziyake.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2dyozgsne.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2wlmbjcdt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2cbzedxsv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2akidvwko.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2smlnildf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2awtpdsei.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2biqkpolk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2vxybclvf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nbytelyj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ufslbmdp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2fkbxnyqg.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2belgumqk.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2jzhnfoaf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2rbkjolur.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2sedtdxwo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2wsocfbpm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2chupxpgj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2qhygazip.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2hvfqfjnz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2vjjzbrel.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2oqfmcodu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2lykmkyuj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2txdqmzbd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qgibeuqg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vwphlziv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2soeislap.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zqnwzfua.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ibprrjvq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2niomtwpt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mkzkzhmy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sfehrxvx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qhhujlnw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2pnmwgcnp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2lxwjojgy.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2hnqgifnf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2geaomakn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nlrnhobq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pyxrcwmw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dprrtvgy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2vdyqmtdw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2oncousrd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ujxzqqxg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qjhkhful.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hzmfdlrd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xhpkbike.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bwipcnis.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2gidcvzhu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2whsfbdad.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2zwzkrbev.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2tgrlwsmm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fdmervef.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mpbewawz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2uyegospf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2upxthooh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2cukkvtso.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fbestgld.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ujlgrssb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2btaujpmh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2gxahqpba.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fbstpwiw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vdtmquua.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqvbpahm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ftqckvmz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2giauynyh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjakfcgq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2wxupysqt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2nofzrjxz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2bwxcbetu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2dmqteujz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ogsolwxb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2htcvrqfn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ujvrspyx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wxbevjns.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vwtxwnat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nifrwzac.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2blxojotq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkbkmahf.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2umwmvpam.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2zkdmirgb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2xwbqmzkj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ecgqvate.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zcjxqpab.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2oxevxrxi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2wglzwwxe.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tiksjnhp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2elwqtcpr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ehtinqlv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2zxhlzfxi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iymghqmy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2azfucivw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gbeqdhyy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2roubsloj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2iaygseoc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lomedohz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yqbycvra.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2upjgolby.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ithieqpm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aketojks.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2anmpbjcw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozmkilkz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2laesikii.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cyfotlgl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qufapinf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2uhokgjbi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2aqqcrfyq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2sjgaxtiq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2uazognhp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxrmvwuo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2adlgacil.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2woocapra.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2zddpzwnm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2slijdrin.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbjomahk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ekgkgjfg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2tecykhls.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wskddsfk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgxhxdxm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kieszvrr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qlitkrkz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ueiwlgks.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2iszpcrmk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjwxmwvi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2wpsljtvq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dyhdlads.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ohaurqqd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nykbxtdm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2damfuytp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvoxligb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2yenfmqbi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2tmvpqlai.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttavicdk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vdsrtzeo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2yzebkdxd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jztkjxqf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqxdfjih.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdazspge.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zqckhmry.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2xmfuuvkr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2cfhdgula.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zivfrmnm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2anysrczf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2jzrtpuoo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jreuobry.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mnbewaox.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lmqttmfp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2youzeqqi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2viazkhkz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vzoqcolt.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tqbebbpo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xzofhqgt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2wlymyehs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxmxtohl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xgftrgof.html


<!-- 参考信息 -->