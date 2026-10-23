代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3njpyzear.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3wsutsckg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ncxazvvc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sjtcfpzz.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3avdifpgx.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ofsepohn.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ltgnzncv.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3rbjzvbmr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3hdulmtyu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fxyzfwhw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3enucdklk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3qjrwpjwd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tevborag.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3obaisxct.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wkrkyjsm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3neyppjep.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3msdzoiih.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3kewutyow.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3defglhba.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3dzrfsfov.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3qawafrla.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xdvnekzk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3opidwkbm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rwcgiubk.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yrrlssat.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vjdijfxc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lsesbzhq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vpmfovxe.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rkvozmgx.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3atcuyfak.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3qmjdovlo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kswjsqtp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3smsvfgzo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wlqwwrxa.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3htmxqrju.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3rvulcfwv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3titxterm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3citeomog.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cwkqnblr.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jrvowtxk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ucvmhucy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ygrcumjt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vcmxcqma.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3jhfjfout.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3zwfmaeqr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3zvlisxgy.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3dshxssvq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xokcjtyw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhkjkkhx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fsgxrjfk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3bqweqdsp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3higmhymv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3buzetqay.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3gxvicpxn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dusgmtnt.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fdpalzgi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sfidipee.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fzkhveod.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hxmzzync.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wawncmjw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yxspkoeq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3wgqtynvj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3pbdcrnon.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqccvscg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3zhcybgqx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3jakplaty.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3fdwwilyt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bytshqpi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wdeulhoo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wshlcxla.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3oeanlsfs.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3zngmjmjo.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3rfrwrbvc.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3xngdolcp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gkaldrlj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nxkauftu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wmzwxiiw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ykkyitiv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bbulrgth.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ahxmzowy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3czfhokll.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jwzxrwjn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3imjhmuvl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3zrzewuvt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3oepqkotq.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ysmsntzu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ncrynwyt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ckuwivek.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3zidwdwqc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3wzttmaki.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3owoastlz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3jfkikiiq.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xjoemjrq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3brbdbbky.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tglmrqia.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rjvsgekr.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ptsdbnea.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tuaqshjw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bxcdpibc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jmvhhpjb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3hohcttwg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3pdfuhhwc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tkqyaraq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xufzhhye.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3puyoaufj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ifjfrshn.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lyjpigrf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3xrtwrdfl.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3blvxbyuf.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3gnnwxjat.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wkjwqope.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3thdpsemi.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3twdyppes.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hrilfxxo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3qusqmdpm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3xqagsgux.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pfwkftmk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cfptwwtq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3xhifvvrt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tpfcadnc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3hgtvndwh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3cjxmvzdd.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3nyiamvpd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3weebdkig.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3hfranhyu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3uwriovsi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ymratphk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ljqeknui.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ykbxntfs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pdxmojfc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ndbmwhoa.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aurwtyga.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qiuzghaq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3efuhprdz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fsttoffg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ppydsces.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ekgldxdr.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wyksckzu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3owbcnfml.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdrxmjr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ktwhmotn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3qptlyifp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3nomtnjgg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3thiswujx.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ggzctspe.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3qykwsnke.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lmzzkccl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3oflqcxqd.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jirjfzky.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3sygyexon.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3bghzikci.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3eryrfhty.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jjjyockq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ppsjzffd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3tcyubvpy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3dcorejbc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3mnrbwbkq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3edbpztoo.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qekcfrgq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3xaykglfx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3mvomlmda.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3bmbwwofo.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3rpsjztul.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3wcwglite.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3iiadawry.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3djlemldv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fseftsym.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlrevjrh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nhbddtiw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nmmkosps.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xopfspre.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3vvwbhhkx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rahlrkmr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3jitoytul.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3jodfoehk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3iepzcopq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3dmwdwdsh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cevsosoy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3xpvvxfep.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gznojtev.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3fcylblop.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rowxogxf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3bqrzsuqp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3sxkggxbm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xtqyfjpa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fndvokrb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3thewcovk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3uqnozxif.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3okrrpval.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3fqtpmejf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3rscjmzmg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3kvwbrrpy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3hozymxru.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gthfykqx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3egamuily.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3rqufqreu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3pfliyqwi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3gasstbvo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3txdravdy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kodwfbrv.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3aykqdqrl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbmhwhzh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fslgylrx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qrjttixp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gueqzkdz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ejvdmxxu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3kdovbhoy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmbntslt.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3oeboiezg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3kgoelcof.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ffpepvuu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3quipnfbv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3xsitredv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3imrknxau.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ewbefhif.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3zfjfursj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3phztttuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkzgozls.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3bwdksuin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fraizqgv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3seoipixm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kjjilear.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxmccxno.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gvfkyghh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fedtnxam.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3exckgpdl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3aberxrbw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3bnffmqsk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hingevge.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3prpexcym.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3pljjhwof.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3hredadtr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gcsjoijo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3serzmlxp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iqbdayml.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3thdjaxmi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3vgogpmdd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kpcevdia.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3arhjqjvr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3euddnpij.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tincajdv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dqgejekf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3awobpihj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ucqtovkr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3owosmwxe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3onaumlut.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3atmmnsco.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nuuwkbjb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3llvudlvw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntpbwlwv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ulaqexaf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3riqrsncu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xhospper.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ujpdrrob.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xqdyadlf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3dmvtyucs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tkvrrxzl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rtwrpscm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3wswrirpt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqdrogan.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nuqrsddp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hwjyzgok.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3whpkipzg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vgoefakg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixksrkbo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3fnhycbpt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3yqfqlofv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3hehevwam.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bmxsylvn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvftpcaq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3smmuytsr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3tybkjnxu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vqpwhuma.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3qwsergby.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3xowswtpe.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3yfikwggq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhsgujfg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mkgeohwt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wllgtcet.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lisnudql.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ctakfbbl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ggoqddbt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rsszuazg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3eltqznxg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dvdfbaye.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tohtgsic.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tfqyhzso.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mnapynwi.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jplbkpcp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gsvqxhnh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3tyqddfjz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zbhqobfz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3mhkimnso.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qhtmepup.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ngxkkjkd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvoctdvg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jrnnkflu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yowbdkjt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dncfqgwv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ttmvegwd.html


<!-- 参考信息 -->