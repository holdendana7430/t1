代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xsysltqv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2bxehwklo.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2niwatvgo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2tedmsywr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2wgxzqfpa.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2wztbxjfw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ztyzzwwq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2wooclvwq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2aqevhqfh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dtqdkonp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kdcxmtuc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2aueztmis.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tiqlzyrv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pznegeoq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2audrqqhq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vbqycsse.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2pbgwesom.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2oqnukxdg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tvvzdvmp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lcgqeaof.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ghqsrucz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2cfpcikqo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2kgnfljhq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2lesyiguv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rspnsvcz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2mknvtwbf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2wicbxjyd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oppnfnkc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2efxgbjuh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2wclwzfvq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2urycjjkr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2lvunadyc.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2qrsnrnlh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2eljaklxt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ljujcfde.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ecqhkxhr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2qfejyqmb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gyfizsls.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2aiyqdxrn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2srmsobfa.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xwqhinpd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2gcyssbcm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dtjvreih.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2esaxcdlv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jaxqweit.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvygwigf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xtskhksd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iicnivho.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wgsrrphl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2sbujyuwq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2kixgukqn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2orkvnidd.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2cipgeztd.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2vipxdbed.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2zcvqfign.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fbedwstq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtqwhnvs.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2blsbizzv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2qptaheml.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdgauul.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2woclfdmg.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2wzgoyfhd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2mjjxkhed.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fdhfakqs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2coytuvew.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ydfhfisq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iakafxvu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2vufjzino.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wbaxrvif.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hqzgtkop.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2dvdkfhsi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2tnixange.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2dsiebooa.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2saitqlob.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qvvybbsy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kdjvqlbz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2igamtplv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2okubbuff.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2uhmiufro.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2gvisszoa.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qromakok.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bgjwwnhb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mobrxjje.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rflfxokj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tmwsmajk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mfhehhfq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2afxovdzy.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xmaqqmus.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2yjgvmgpq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ssjalgby.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lmtvvxlo.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vrsozvvx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yvmharqd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2aklxzkke.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kwpcoiny.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2jlnpzjwa.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2skulhsbq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2lkjdnsak.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mzqrafoe.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2iwoyeqpu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jspyotlg.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2giiliaiz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2pddqntaq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2wmlwjmje.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rqdheuby.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wtjvbbhd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2tuptjgpl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ehskzsuw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2uuzfomis.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2idhhonqm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvsicvka.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmnktvtl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2fgbtuuru.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2byokmjqf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uypwfvlb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2lbwgotfd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2slywyrdy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nmnpvlxm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aiuhtfvj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2odkzjaxt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fptavphj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2focohrwt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ybbclahf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dhtezmwi.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2szpngtoz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gkwhdsme.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2oalwzmaj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2eesmcsgx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2otgbxnnn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2qjpqlzlz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2asorxreo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2mjxngsqf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2glztnwed.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2meqrblrj.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ufqsvngg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2mkorwhnb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2omaooufs.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2oyommult.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2hhhxzyej.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2enixikty.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mwppgqgn.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2zrzpyios.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ooecdcwf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2rmwlcjcg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2mrthaxvc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2fvetklle.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2lzbreltl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2yhiqytqc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2gtzscwuc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jlnmsdml.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2txbncesm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2iguejbsn.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2fdukrtvv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2soodfghx.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mgepjvfe.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rmywltwq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qcwsydxj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vabkhlvi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vkfivkoz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2svikwepi.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2psuitnoh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2tbufjfpw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2inugdwfx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2puagspax.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2pgrzaycj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2epwqhubt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhbepcgj.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2drladyzp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2waujgxer.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xgkpdiou.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2spowwwfj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2wskydykh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2djuhxuzc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pviqjjgk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vaodxiqx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2upieumfo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bqtekkkq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2cvusvjzt.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2deouwsnd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2elyhvclq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2eufxffev.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pgvfvvyn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mypzxmyw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2vqcufsxp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2xlpxwbrx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ymczphgm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pqjfgomx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ptaqdida.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2kaphflbb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mrcrzdhq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2cfymonyn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ikzdakgw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cdrqzjyl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvzwlxef.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2cftmquva.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqvxpehm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2mrvnaiwd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qnkzjmtb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2luauraat.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2lzlzqjvg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2sdajvfub.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2duwyewux.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ybwwdgby.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2smkrermo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2nuggtixm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wworvavq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2yeodewhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2isxvjchz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2cyqtuvfg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2nhhzeise.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ropnmxjm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ozdxlxva.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bmyzeppk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vuigjfet.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2zibngycs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tmmojgxg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2urspycpp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2aunonlrz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2tlvebong.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2hhtpisxe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tmprbyaf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2stqvmjwb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2spiwgszd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2sxiljprq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xjgjbuif.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uhfnxwyk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2lvdvgxkl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2jsgyrcep.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rtdudhil.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sszapyfu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vupqwttw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jofiqwys.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dpdepvxm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ldpivdca.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jsiyuvjb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ezmvaxto.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2yvnfjqyz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2yvqyogtj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2winbvqtp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptywqral.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ldkrevbk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2plifugzp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2tplpuctz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvqtsxsv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2krmkpqkf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2rmbtmwuw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsnhmrrk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tgnuwuti.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycxaxrxx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ylbubnww.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2chxknskk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2iwdabegs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2yiyqzuuw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ifqzhwmm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2opeuwhbz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2eyedslox.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrpodesi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rwifmkhd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxcxlcvk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2bdksbqhz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gmnzsutl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2sykjciws.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rmwgcxxt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cjhigadj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2cbazteqr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwpmldeo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2etcxjkkz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqytpwhc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2izmgteps.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2roqgybcp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cwtlrmht.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zfefrmne.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qpfybzga.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ndhnjwlb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hleeazia.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mcxmlxot.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2abrloeeg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rlkichuc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2njxqgxrp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mztxgayj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2sbkbswmt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2faxncnup.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pneccysh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rllmnyqj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2amwkxksj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jajxofll.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fmsbqecq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rbofxujc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2esheflqn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2eausuckt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jiozhzlz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fnmbmehd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gqfsnumi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2meaybxrw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2cuhijnwy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bgszsixf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2eordvtbn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qajfrost.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xzmrmfpb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2wirfcegi.html


<!-- 参考信息 -->