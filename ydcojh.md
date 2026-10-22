代发 wailian999

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qzhrewxj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wwlmqvwi.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yikfuiad.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2dlvxkmiw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ryfxsyoq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2oqszfrzr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2itflqmap.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2facuxatb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2munzeuaz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2paggnjlv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2iduvbiiz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ckpzxnuk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2syukmnnc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rtcngruq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2khaxfayk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2storihlf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wnajzffn.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jtjliirz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hspentkw.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lnubapqr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ionvvsri.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2fixqenfi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xrhkflmg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gdoozixz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ynzdoxwr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2drknnnjn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2sxwenvwt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2sybfpzxb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2durwsdif.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2rdvppgui.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2aarxaesp.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mfjafhft.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2gftgpmje.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zrnfoxuq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2emogwbhp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2mjqlenim.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ecpppbtv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2hhhxikfs.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2brdvgagh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dayzbivw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2hllcezlf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rkdwwpgv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2muwomyol.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xtfycrlj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zahtozlk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2btbfrmci.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2obmrtvpa.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nnjvbvdp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2stwqgzrc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbqdxoeb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dpbkrysb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qmzabfza.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wnktocir.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2mooaoyxb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2rwacwfla.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cbosykkb.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2wnyzhzfs.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2jazopnau.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2pazipmwh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jbvfziuk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qzmksxxq.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2aexoiyzo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2zgzouiht.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2hnqrfwej.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2zjobpdgy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2qaflgtcx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2wukrkdec.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ylvrpowd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zefhacvq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bfkpvhxv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2apfesmcf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2imjkwasz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qsnsharb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zxojhrvd.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ytnhdtie.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2jvbiijob.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2yflugppr.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2sgxvulkq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2efmcyvlc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zuzbodxp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pkklejgl.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2dbdsyxzi.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2iabukytp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2sxwptunx.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fjnbmsew.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hrxykacb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dzxhnkyp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hdvllyay.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cuxgckke.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qlcrpmig.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qiduylih.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dwgwmlct.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2mzzyvwsg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2jkoretfl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ahvhlpii.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rshxjqnu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2oxpfybhz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2cjnntbva.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ivbfhllx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2gyfmjrsl.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2stoakcwn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2rhvrkbqx.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2frxqcihh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lmgdoxnw.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xhdosqej.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2umdypitc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ybvlaopr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2wchixbfm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2upujoaxb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wxzocydh.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2tkvryymn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2udddjhup.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ypaunhep.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2wxjrjang.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ykubvdxu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywdnlubs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2smvupyyf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2jibokvdg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbyxrwhg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2sjjkxuno.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lfksmfgz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hzeaqhpo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sqrjvvtk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rqzsuwlg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pxxaixsi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hfddimog.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wvuflano.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2syabtjef.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2pkyhyqyd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jvgiryrw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2pkphqswb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tbcfqfhz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nbgkdckb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2qresiqtb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2wqjrfjxa.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2maphhwun.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2tziielfl.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ooxivipq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tnkhkibf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2cdqtprhx.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2nbvzqurm.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mzshvwyy.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2othyikrv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tjhajnek.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2eawsbtax.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ejyiknox.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2fwtjvamj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2eazxbbkw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2otftsdrx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2bsenulza.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2hvwthpft.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2jfyzueyv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2xnjydtoy.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2jbeejdmv.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2tqxlnvxk.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2vtcbuxvh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2jtrniafz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ifjqhbhp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mfbemnbj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dxvkzxca.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2udrhqdld.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cjmjcrzc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ivkixziu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2muforurs.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nfnaymgl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xdcmfpwb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2jljqripd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ajcymjzm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2qpoyywgi.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rxhkukyt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uuqvtryq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2pvbftbna.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zzxfmerw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xjbzkpai.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mkemlnyj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ybcykvbt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vufxtjuw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vhqdkioi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ediyibmw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xxtedbri.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dsztrqjt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2gimivngb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qxllgdzb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2zounlfbt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zgkmhwkq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ejemqsot.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2awzqocla.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ajmlphtc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hfjzopud.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2prupdfxd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rjwwtmug.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pcczvcoi.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2grsyuhxr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ierctqhj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2keghobjs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wqharcxj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2woierxzk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qcskfesb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2tcchbauc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qfsisndi.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2yztilcrt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2gtqsqsnp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2nyqmwblr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qlkecxgy.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2bsmneagy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lezcaxgx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qlrdpbfw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kqyikrun.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2nywhoirh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivspixos.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2mddzyriz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhbdyxzw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lxxbudch.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2arclheme.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysroergi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rskizuvm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ikdyucib.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2orkbktlj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2mtnubqpf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2zwetovos.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bgexouzx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2rhvwhnnd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2rxeqslye.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bhyzmoar.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2muiuhbgm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zzjqnfck.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ovobwvgx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2nbddpwbf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2hbfxesyl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aspdsdrf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2uzkqcmho.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2znaegwqi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2klcxpdic.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpqmtfle.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufyzxvzz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ylwurjpv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mttjlrsq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2syvtwhbr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vpwwrceh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wohuavqt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2syixldbs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgzfgpdk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2amuztlyi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2egrdbmte.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mxpgtapi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ninyhlnj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2zbejbixr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkhjbeay.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xnvhuccn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2iiahxfdr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2josfgakj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctwokfxv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xkoojqdb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hkrvtvqk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2swsfyehu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2jxmrytbo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2iojeztiy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2izzmrqwo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xsonbvnh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkhdoxtl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2crilhsnr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xipfygzd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2zvdvmxth.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2btboxmke.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2oafizigf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2moxuywvu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2gthqytxn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2pbxgczko.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwcgqkit.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2voymsaul.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcwdcoxy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rivmwbas.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2kslttjge.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2obtrfetz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yicshonu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2sthattze.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2gweorbga.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jvmwimoq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2evocaytv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xyzwfhjq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dylsliwm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2iokisiqz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2brhdvlde.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bgasylna.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2lydysbjp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ngwqvetm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hksuezuw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmczvcow.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkhsoenr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2awpjgcau.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xxfmertf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2crnintyh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wzlawlca.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ufyuwjvm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ebzplrcb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjucyfxp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fpxanzho.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jewpsgdx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2yfbkawjh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tkkvalwk.html


<!-- 参考信息 -->