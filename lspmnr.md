代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2wexgtgwt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2njebywiw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2agglnngh.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2orlmkhli.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tfsfeiok.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2samaedbs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2syratmlr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bbfifiuc.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bkrqeupx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ezyznobm.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2okvwhids.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ccdxssno.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lhkenmab.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ksnhctgr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2utpnuwys.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2hvjlagrf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2phrfrgej.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kkokkpup.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vumyzzcc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2cbylwnxw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2jbadnlnf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2fzikdsyx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2bnifxfar.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2vtdsqkqt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2kfoimohc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ovwielli.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zukgrwji.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qcjzglaw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uiilkzzb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2oaruhxni.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kvutlpul.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sxikruyw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nbnrgovn.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vgxjpylu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2onyeykpw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2joctlprw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xbbhpijo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lndbgwfp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2oliagmqp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2mwopsdsd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ptdyelgo.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dozskqux.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2czxtbifi.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2gblofwkc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iloecioq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2yistpgya.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2tyroesfk.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lipqdyib.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2vccnehbd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hpoqjsri.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2qgexjcau.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qmtqcpxd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2eoscteuo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kbtvsotv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ulvdklpf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mvjaiqls.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2islrqdsd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2sjzmnxen.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qeccpgap.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2imluxkys.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rfhvwfvd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zbvgsofk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejkjsqpd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mggufglk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2leebgujx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2jkuvuzgf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2pxxxbxvq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2obzdsniq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2agprjywd.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2dxdzogrc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2bksuumah.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lpzemvko.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2siocfjab.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2accctgof.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2qbtotije.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2amzrvyjs.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2yzlaerdo.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2osmhrdrc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2jssoemhb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qnymlhsf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jgfchmuk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2opryvdav.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2onzghmhq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2zarqlyke.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2amajkfrv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2adyztsrq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zcyolgmn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2cgrhvigf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2apdiesfv.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2lpwpstui.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2dcxohneq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2lloedacv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zpeebkbk.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pijhnhjn.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2xmllnljg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2qxqjhhur.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sojznehi.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qcfgeflg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ciyulvam.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2raryzwbm.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mcmddpuo.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mhpavksf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iablwmcw.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mrdlkrha.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ntuonnpx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ktzcbanu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ydalltxq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nsihavev.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2frvqicyo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2aesrhmyq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2skayfpff.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2whqrcutw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hidxdbih.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2vhcnaros.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2vzidgosf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oykzcqil.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bfptpjni.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2serkrukz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2sbxvnwbp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2favcnavt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2olybfoas.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ccffnvzi.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2dnusfisw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2tyvfvcjk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2vtsvdwpc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2vrrgrzha.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2wcushyma.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wobisdos.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2vveibtdu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2qrjlzezo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xftaiszx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2zifjodnk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mslhsfpp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uzofduxx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zklnllyb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wegxbbug.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fvltvmig.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wcukhfqf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xtsnijkq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sslggrwj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2gqavmusk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ojgrcdpz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xnygfciv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2odosviij.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pbfdgcwh.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ytafxnrw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2umrvvqil.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2jqtrpeix.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2agqpauvp.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2zamchfqs.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2luvdyqqh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ncwnmobu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qwudmfup.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nqabhcte.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2vmtrgcps.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ochzqhbm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cewohmaf.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2fbelrlqs.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2pwcpfcqy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2icstyldu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2erpvnnsj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2jmmtpfxw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2seecgnfm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2kvoxxdet.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2gxxdwjni.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2uvhwhfse.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2uyrhmqjf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2vgmvxzwi.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2gccqcvys.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hcjlsvkt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dcqdfeul.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2eankpjqh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2watbkeek.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2iantgguz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cntmarqz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2kjhpouer.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2flrhjvpz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2hhariihb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2zjvhjbxd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2naandjmq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2gzbgwaeg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mzkyramk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2rthaguyw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tzmdogbe.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uvlztlql.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2aochkyzi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ogqnyjca.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndyzrndm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2guqrhjri.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bzzemmbc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ixcvjasy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ezvtrzpi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nxrykzwc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2qgsulylk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2bayzijrm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2nwdasnrz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2mzovsxwk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nrhxnbdw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fegnbqpz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2bjlzwzqw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdcnitjh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2lzqxpvbn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ayepppai.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hujgehig.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2kyzfnbzi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ymyfrqvl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2unkihisv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pwxrupdq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bsadkkcf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2swxilsis.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2lymqzkxf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2httoavrx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2xicbvauc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2uiprabfu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ztlddpiv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jhqffiwj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2stzinitp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dkaicvtf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2uisaqksd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2wuzchuju.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ukqrfpwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2veambqqf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2zaxchkyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nryyewmd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2bnhicoog.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ipdgomhi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2vdvxcxfb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2stsjbmvb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gkxpgpjo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bsmoxkdf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2jpdcxdqd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2sytgrhaj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rtcrqmnh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2wnvarwcr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2iczxpwsj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aldsdabj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kyhbdqej.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rryqxlcq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zinggnor.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2btkyihgt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2kalnptgl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lfkcqzdu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2knodtcxa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ifkzhlhs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2apjugywk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iixvmnjr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlpzxlym.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdnsezbs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gusmdqtw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2gjjqufyp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bznqsajf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hobcaipv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vhsersls.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hyftabdm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lxowsnew.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppatlmub.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jlvcpham.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2hmasxloa.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2sxlfzqzz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fqvabcei.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dnykbykv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2lhngfxba.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2mgvwqpse.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vafjsvnt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nzhdohrp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2jrqnlpkz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2emoxgzhg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2lizvvcae.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rmmuduht.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2kqdxbzcn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jmzqerty.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jvicrddx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewojdhxc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xohmaglj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jpkxghih.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xzrovkti.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2zvdliylo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2diqbrcyi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dhqgcihw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xvjekhkr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rudqnodb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lrojpghx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rqgrkycl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2giihamgd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rhhgncuo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2rlyxxlkr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtdcznvx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ehgyhqlz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2skeemrkf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rswjiihz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ltfcoxor.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rythwbbq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qwphzzfy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bieplush.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2khynwfdc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uefloyfa.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2elzctsha.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tciifgyy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2camjeuut.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tleuilfl.html


<!-- 参考信息 -->