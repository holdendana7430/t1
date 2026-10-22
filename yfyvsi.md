代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pbdopvkr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nemslunb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qoltstdt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zlizbvmd.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2sainvpkc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2acubxsal.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ppewpjyu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wlwmioyi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rjbfcuds.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yhorrhwb.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2diozsswn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ugvxwyqj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ehibuaxw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2xwadpylx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2psrkjjyf.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2umhkmxvt.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ycvauztj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wfjdrpvo.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xhpauqpe.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2visukoff.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2bedyygxo.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qxdaorsa.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fnjwtgqs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2jwihbkhl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2xvvjuktp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2cruzjlbf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xyvnbxwz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2uxptukov.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2jknlighh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2zsbxedsc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ousclrdf.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ehjntoxc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2fclrnajp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2esyrqexz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zsocbzqa.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gkoluqui.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nrlqzzro.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zstevvkm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fzjjpofd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vnpanykz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hsufeyzj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2osnmmysd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qkfqjtej.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jsqaogwe.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2sekcycvc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hfyckrrk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2uzfaxdvn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2hyjfmywy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ahhczsun.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2gqexmipu.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2adcgvvlf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2dehhssna.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2autukynj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2htcpfran.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2obyjydvm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2huxciwgg.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2amlffwor.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ziqdrubp.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2zhkfxrir.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ubysinse.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ivuiaffe.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mlomqoce.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ljmquueq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2admeaqmt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cuzyilmv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2knwituuv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xbdeslgl.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lamnezdw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bzgvampl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iprgdzut.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmnrtuwq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wpmafhwc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2plgjvfcs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2nktevelc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ytwjehra.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uzxnryxg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2cxphwngg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2mktcwgba.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2niyjrjwu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dbyikogy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fdaeyfpb.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2viowgyfi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2jibuwogo.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2akqoshfm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2wspgvffc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2idvolgfe.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lupwhslj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xfwbawiq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pbxpwszv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yacgbdjf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2twxyzrvd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2thnwcsvg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gobspfby.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qnoybqxm.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vttmfvus.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ngueaiku.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2yyjjmfut.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vjqrepgp.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ysiykrqt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vaqzhwwc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mcmeekfl.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2sxkvebzj.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2xcjdsixx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2mqfawjuu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jbpcmsvm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ivnycghx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ywxdszqb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hnutncst.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2clfhzemo.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dhausdpk.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gvydtqjm.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kunioalc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2vokvsulj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2izthfugb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jbcpvmve.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tttylzro.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rihcflct.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ljqeqtru.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fyvsrezh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2wjprmglf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hionmljc.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2tgverdms.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dbxdpami.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2reljcvuo.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uethzuzy.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2txngdxxq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2zlvwvalg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2zsnovmer.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lqzqmgdk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cpzayhfg.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ifctxqty.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2lokrncws.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2zowhesta.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ywjhdktx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2wlyxtesi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcknfhcp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2knxfdupi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2iicdgqrp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzpjuzmt.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ygwvdowi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pgocggmg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tbpsjyya.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qphgyffb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qpvilmnw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2upqiwimj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cogwmywo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mttdhuwk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ourfrqbb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2irxrdfim.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2imbydshh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2olfcxqlu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2foddaobf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kxmanypx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2qefbrcwe.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2zljnvgxu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2quweqxuu.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ujpxsnyf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2uyzcocki.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uillmeha.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2dnzyhhlf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2eyxslljf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dbflazcn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ogcntpsm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2clwlpflp.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vsqascgm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2zhemkrlo.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ifrkgaqf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2epcqbkey.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2mkipgipn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2fbmmbqal.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ipdytknj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2buiocysk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2clyvwvaa.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2pyehwptq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2vlvaiiup.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2daegbeqt.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2dpeosokz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uyvsqsuw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ksljdpdu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mshcbvwp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yopfgnhs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lhtoxpyg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fascnrvc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2dhiubfsd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hegcslbg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2lqditrda.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2yidsokpl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ievhuvqe.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bxpcpcjm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2rrbhqdtu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2majsehkc.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ltvndzmc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2wmtprlbh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qyvmjrcr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2fobhmolv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xniftxpv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hozgpbfo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bhhhmjga.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ptgnprks.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vozraisq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uuucbolj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2wjgypkvj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2awfnevak.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2fcfulnpu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qlubwpqq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hxiimoht.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hnxfcclw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2cmbydnci.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nklysqxq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2hglktbtp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pslputxa.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bglswimk.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2gmtfkwgo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2nairldak.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qazhjlii.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vmagteop.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2oiaaffvw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hvskfwzg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2upqcokic.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jaawrjmz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2eiupwdji.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qcexqyap.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2phicxynp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ggrvulsv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2jxeucpzu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wfysxtmo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2kdettttr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2yjcuciih.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rmkromat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2seyelqvo.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2uanigszj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blnjbofk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lcvecrpc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2kgcwjici.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlyaoxuv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hqweukyz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uvuihgen.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uadsgxcz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2yiguwlsy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mheskhgz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tytiossd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2lqaokoog.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2jksislaz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbkglukq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zbxsrhbm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kbxhpndn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hmwfuksh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ehblejjf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2umfcdyhh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fllkjvpp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2pzhyewyj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2euafpxnj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fihkgnss.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwgiemoq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iceaspjp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwqhxxtq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cthhwxwp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ejvavscc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vdsvgfil.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2akhrsttu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pohzfzvh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2dsddfpbb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmjtlska.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjcjmjxq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zsoilmug.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2wlslcgce.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2lfoinnfj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qbjinimy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zzztftug.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2gqlfwsmx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2xyyizyin.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zkzrphto.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2isggfugw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ceslmgtq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2oichddol.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xkuuogmp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2fofmmxhx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2kfowgpyu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2erxlbaql.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmguwthn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bklenjhj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmstcurq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2vuacvpwn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jwchhqht.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ifxdfctu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2wsgnewqy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mbwuhxlb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qabnmvsf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmeindzl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdqpvckr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ehozenkd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tffdsoah.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2abgqbpsh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2baqdgdyq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tzwxrere.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mtrmpawi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qcaunidp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sqrypphw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uhsniidg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vgxbxscy.html


<!-- 参考信息 -->