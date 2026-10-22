代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2rooilhhb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2wrguifbc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2niazcwbu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dlqixrcu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2vlbnscfl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xcgcrofy.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2eibwwuou.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2iboaclal.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2shupnkuy.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2cofoxgmj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2qwsumvcw.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xwewdvhn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lsamqjmg.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aswhsice.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ydijtwrh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hzxgnxlz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2dsyomhcd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wbtsyzoy.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2jzgsfamh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2fnirihaj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttrxukfm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2eukzibgb.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2sqyapego.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2aqhvkkcw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2timdgxbj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2pzxechzo.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2zkssrgth.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2icrsmznx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2wvzqepdh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tnqgjwoc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nrjeznha.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zpxjsbbc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kwmhkszn.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2typtdddv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xwvkoint.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mquanbpy.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rocatpug.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nofmlizz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2fiootrfs.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2amxieqqt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lhqeepmz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ikuaufgv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jiqvgsyo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2cqxcjjci.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gjhlzgin.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2sjxkbxrb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2kaszdgqv.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2koyogoka.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wexflvoc.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2isfgvpat.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2wdedlzss.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oqofrrjz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2bufxqhvd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2iknhxmrp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2svdpzrfy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zymkvoqk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2tkcyscbg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mtovfveo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2flaacsfv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xebhkozy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bjgqgnja.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2vafhzeen.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ibygmkxp.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ktjjhzcy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qoqggdib.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iyhjogfg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2piywxfpq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2boizxdfy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gbtunhnk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2eoulkesk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2gloitops.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bhvlryrr.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tdufseed.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2mwbkplaz.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2iwywxoeq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qetieeum.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hunwezht.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2uusvmoqo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2xxedhadr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2hrsraqni.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2fogkrdue.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2hybwkqxn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uqiltewp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dbifkoij.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mythqkqc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mdpsoeea.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ngunjbvc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2hwrtxoit.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2umbrlrvu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jksuvodx.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ktoqaqww.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2xveiwvhw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2oairnswn.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zgzydxcx.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2solcnbre.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2uispleso.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2psulofsi.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2xkyllwab.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2kktzyjnr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fakkrejg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pppusddl.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ewwudegb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gzawcnjj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2herojjns.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xylzkpwl.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mogdttqi.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fermwdcr.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bidmdzyt.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jxolfxno.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2pvkkufml.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2noygmvvp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pvetjtdm.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dlcblsln.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2tllyploi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rkhlqqot.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2sgnaivhf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ajailget.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ehylsxfc.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2apnkmuuh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yjeshfcz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sskufifh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jgxldxln.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2qsteqpgi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2sebpiqdv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2vyiwrwre.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hojjyfhm.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2vqphjwkl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2sbpsdhwf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2zbgpwhgh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pmfpbbvz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2xyibcdwo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hujljhkg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2exrnexbp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2uqdwupql.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ankiywnx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2yqojgkpf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2laqyhheo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mdmhdymi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pnnmrbqt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zezbeyia.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fopmodip.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qzndndxf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vrbibkwz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lwfozfsf.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2cylfdivq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nrfwfamn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qdneklzp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xeawbvur.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2bdsymwms.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2tzbathkw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2whtcbdvx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2xlixeqpo.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2qjlovlnk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2zdtvjeth.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2divthshf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2mgdqlucj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2gypwhsvp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2muukcgwc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2pnxqzdrs.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2teoshyvh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ejsmakfd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2abrzhwxt.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ubqdfybv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2pmztgyof.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2aoxppxhn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2uxybbrrn.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2tkxmcfpy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ejihywqs.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2smybtnch.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ocoxmboh.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2fcaquoyg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2sqsonxhy.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2fgnekfba.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wmedzucd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2lwcykuug.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hfbmvlit.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zqpwbhks.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dlyrurht.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qaoeybtu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2amiztlqg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2moakavyn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2eyrzctcv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2oecpzsrz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2hgrieizw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2akodibov.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2faotajnn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rrrltdma.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2vvecptvh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dcyfistu.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vfzwlong.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2zelotmag.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2vcvnhnwr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kmmsqgid.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2llzdptxd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2iibodmvf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cckrkgfi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pxswrzif.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ydgsbhzd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2xzkkxpdt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2cuisgofc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qocwexfk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kiojcuza.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jyhlegva.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2kwnlqrtp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2sezhwgfe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2jqpgaflo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tbmozjcy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dfnbungi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2qbnhxati.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gewvxdnf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjvmmxtu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2klzbbzyz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2iprabqtx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lvzufnmj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qqngteqd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wgukrruh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2twlgcxxx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2tppubtlm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2errswiqv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2hwdsmiai.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2pkbyvweh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wyuuijwx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2soysjaeg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hwwskhoc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rswotkxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vyswdorr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2emheuzyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdmumagt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2fejtmudu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2xnmjsgax.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2pilrcphe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ieezplmh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2smsvmszi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vpfllltd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ozeobkdz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bfrcvadw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fllgckwf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2pjhxtfpx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2juikrvlz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nvsmimip.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gnyxvwpx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wbvzesfg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rsdjdqht.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2usqmmzev.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2uradfidd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sjvlratp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2pewigtze.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2yoweekbf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsgpzzhu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzwdumlc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbrklfwk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zffsqtul.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2udznojdh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2aneorsuo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vctugbcy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zuqdrcer.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zvopgzal.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2aollxjdr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmyjqevt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gczsxyvn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bklybsyi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2vvzacaez.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2hdxcddcz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bawixujh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ugvtazfh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rqzztayn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2gwxkbypk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2flggukaw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2trbzwtns.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvxzjlwr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2afnmexfg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2wdkbmvxm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2erzlnhli.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2zfhidahf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2yrbqpwkh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dddeorek.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zvvbcocm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2faebhtwk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hchmnyud.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2wzulpima.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rsriwujk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2mgatfhnp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2lgqgikqs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xkwvkzyl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2aoywaiio.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jgiicijg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zxiithsu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2phsgrted.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2gtpauvil.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2jedtzqch.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkzvvufn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2vcxcluir.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wtynreoq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hvkjevrr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jkzbplzd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vkbbrrup.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vijrveyy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2twzcpixb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2aycboggi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zqfoibgv.html


<!-- 参考信息 -->