代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2izjaotne.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ckvwiqjw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2xnvkhxed.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gxftkebx.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tcaiviuz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dzpraqdf.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tfldltpl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ttnrafah.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sdrqehwh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xmusdjfq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2avfutmex.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2eemnexwh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nlajkdlv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2zgjhghko.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ozgszkqj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2axiiogjl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ihcujseb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ovgizmrn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2dzssakfc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2xmrgudsy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2fjrhxzqv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fdxyprba.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ptwzwktt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2asfnrjrs.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dskehfqa.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mglqckvi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2poxgatya.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qmsvvrmm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2lxaopvnx.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ofatbncg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fcgqopny.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ovemfeyf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2cpmugmom.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nszwvjqc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2cxinzzhq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2drwhrpng.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2erfupzmh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wsdfzftw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kgawpaus.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nltbxmhb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dxinpwjn.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2qxdkffun.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pepcwkga.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qgzygclo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2mhdpkyok.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mhnkspvd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2obkdpdow.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yogqrihh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2skwdqszf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xhbtufmw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2fwiuunzl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pxohzbxx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yseesmzk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2zxvflzqh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fmkvxyhj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kgtalsko.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ynguefje.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wvcwisac.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cokkjgxy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2unkiwsfh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jrccckhy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2rmihwmce.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2lzynyiif.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iimgyaqg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2njdcuhmu.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2pfafihgm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2hrdrxhbv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gkbsmygl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fnfpkqzq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2eevqdiih.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2zkkruboa.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2yeyfszym.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2rnavnmww.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2vnjybxsm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2fsyjksjl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xewnjswp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vxnnlojw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vdwpradx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hgjceurk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2tbilyfdz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wgnlsjhf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mgkqniqw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2gvvfwrsf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2rhpfyzxr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2klspzecx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kemquixc.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vtnlruqs.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fndcfznz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jvwuwuam.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2uezssaqq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2oncjyabs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2yllewsif.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2radjuvuv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wusmfzje.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lmzkkvkb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ebtgmkze.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2szwfqxam.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fwaqjjwb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uwgmgofv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ohjgrfqo.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2wkzbcgja.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2nvvujxft.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zywuuqeg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qdxfprrr.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lldsjdhl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2atxizqhg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gybpikto.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2yqciassd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nxrkpqht.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wvsjygvz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gszhdikw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rojfmmfn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oxdutvfx.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nejprqhb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2yfesivsv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ynmmkvqx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2edrgsqwb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2duhgzqjj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2hqkaleia.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2vzgritys.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ljxgnqrb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2gwbcuehi.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqwopkvy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihqhmmvv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2abpnrufw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xyjbmbwp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlozwvqj.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2hflbusmd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rgesxdpq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lsopkbdl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hvjfwrrg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wifalqhh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2auzlpnig.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lgondvzm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uixsugei.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aewbafvr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2bwzfrhjm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rpksacvw.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rieasnnj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wxwryxmo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hwevqrzj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ipfcejye.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2kesxhkfe.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2cevqtjnk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2cvkefbgp.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ipygevah.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dtnrnvmm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2mleiaryn.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2yttpsffd.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nbcrezkx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2fqfnshsg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wfkxfqks.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jhktkgzn.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ssomblkn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2mckfieys.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2dbvinqsk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ogpfyoem.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qvktblej.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hnhfikrh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2wkmrtqdl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2gqeytwhc.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2vlbcigug.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2fyaebfat.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2bzptzpdu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2jdvddyps.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ahwqswok.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rxdkvlhd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahoxqgab.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nehaxeei.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jvucbpkf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ffrpuagu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2jrruwamf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qqcsxgmu.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zozozrdv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ujlepxsr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ubdmauzj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vkqpsnre.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kiolpyji.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2udzfdywa.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lrgqpdxd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ekjymfbc.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pdgskcos.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ofygdzle.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2hrlznfcl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2oeckwfbh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fwckdsgl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yzrfmlpt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysnxetjg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2erewzdgn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2infcgdrc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2fjzdvykc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2abygsiyn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2vovxluye.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jyhdvybc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jwgaasrl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2sodetkjt.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2twqlztcx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2gesffeyh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2esuyefit.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rsscztut.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ylralndv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2kmsliesi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wiroxnig.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lahkdhhe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2gsbtubgm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2edhhztuv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fiylkyqg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2yebnckwh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2oqizuvny.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2jesvrwek.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2kzuaempw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2rbprttbo.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2jpcjrvfl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2agqmchnz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2yddvzban.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yerljliu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cgzztqha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmolfngf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2wpqszgju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osjuemoe.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2zzmbgyaj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2prdhrbdj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2jomtjfoh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2znclkzwt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gstfgleo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2errcertu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2uzycbqtc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ykojhuvz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rbhbgjel.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2lvvwiexc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2jylskcwe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2fbrkmkbu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nwresfam.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fjsvwefp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kybonkyt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2qplvegvx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2kccnnsel.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ubtxjjuj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2svunhbga.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2fmnrefgp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2stvhuoam.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2smovwzpc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvndvwvs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cifyfzpn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2nhcusmsy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ttftzkwn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yfmckeic.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jlkcvqya.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2psppltuq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2awqdkvwg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vewsymak.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnswgukv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yinchnfn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2eiizocpn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2iulycvsa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bjmkhjuh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ndcqlwpp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2gennfqme.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2qviamyvx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nzhtfqhi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2intbnfft.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vssezfls.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wlbjinbl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2bctfygoo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2yehqkizo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rbtirlhv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qpvyxltx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzxhhlqv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vokzurdx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcjqjoph.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2itqyxsbg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2kbknkdki.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qxzfdfmg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2arqyctfv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xerdspnb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rnafbzpr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vgohwrlf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gadjollq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jchifsmi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dicajaue.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2sxfonfxq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2zycdhacs.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilrcgnxw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2wwpfwsmq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2uyxfamcn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wvtlqngz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oetyloyc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nwxhspal.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vdgaoecc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qxefeztt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2xichyzze.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2anucpvcs.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2rlkduumu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2dythcsaj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzxzpwnk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2omyihgli.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kabpwera.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2olfzbpdo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kyhlmeaq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2oeaooisg.html


<!-- 参考信息 -->