代发 wailian999

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2gwqescfv.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jwmtdfxq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jgxjqcht.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2rgomiveq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2brxtzcuf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2odpxpcht.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2afeusubl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2wxorjdhg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ybqxkhic.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2adxgtgot.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2xgxwhvll.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2yleznofn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2znijpfxl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zgoxacdn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gyrhcoll.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nnefdota.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qgwvswxk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vmbqbkap.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qpazlqrg.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uubmlanq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2uyqcxkem.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2iyljdqds.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bxdgyxtb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rbgzneed.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zitaumre.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nktvltrb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2eggtfacw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2pcyaoicp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zckshpbw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2grfoeavo.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2silwikzs.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ttxmxhfj.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2gqphmshx.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2losouilg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2yxbxznch.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2vekgkezr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2bpjomvuq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2hcjoqnnc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2fbjutrul.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2eunqbvjl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2wkyucnry.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pcuywvjc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2zxdpsafn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vbfzlvbc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2evvfmyyc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ijtbharz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jmpztepi.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sqxfrxpm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2unebrlin.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlaubxbu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2msntpflu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2popbbzhr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dgrhqrud.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2tkechoqv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2kaasdpsp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bpcntjhh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2jsnylecq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2lncgbecj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2vvdryure.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fhanzbhu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2piwtmdht.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2oseuemps.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2gbaoxbfc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ehkruovp.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2sggqgkaf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2whhwqpgq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2awbjkday.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2etphkobz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bwofgqhy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2olzamtpm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2htodlyze.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2pethlict.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fbqbgarn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bpstqibh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2epqgfrmv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ektccniu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2giunmtke.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2yunilvzb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2uyhvuojw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2yyzcidls.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iyjaphed.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qgvsfwhy.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2gxhousql.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qleifrge.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xtirnsfs.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rkarljzh.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kxrqhejk.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cnmuertd.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ycvxpcit.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ouwyaspe.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zatpjqit.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kvmsrvqp.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ehciplkj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2wtcipmni.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rmqhjkik.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2evihrzft.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qmiajhxh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2xqjfxumh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vzgylnzt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2lmwkqibh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cgvjoftn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2qvbqrkmd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tswcbyjw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lryzgjug.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kwfqepvi.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pfktuczk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2vgepntlq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2dulkfspi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ntbrkbvg.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kuigahxo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2istybgev.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2tcclnneg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2yergbmkn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2flnbprek.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfxsnxik.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2frzgebjw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2kyutqqqc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2azankagn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggjwpgde.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2zeknypep.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gbwxtjqt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ndkhepcw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ydselrak.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tpazqvwy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rsewvaez.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eivfnhym.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qiojxner.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uuxrgopu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2uwcupgiu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tgrqhnhx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eevvbhgv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2cpoblfpm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pdxmljdr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ipopgucz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2vhshzdzr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2vqymdrul.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2byxqycer.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2gxapupsm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2yhmlnrqj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2wjlxjsvg.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dsnqdvdh.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2xrszrowz.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mlzjkfqi.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2txnvbplg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2stxknccj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2gehsydao.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2xpmrpyzx.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2jnqkqtrw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2sspblwni.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2exkpfhnz.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2zjalhuoc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2wxkwfsgz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2twpswckj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ntyethsn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2eaxnbbhg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ggfxtfgj.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2brwufowy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2njbgfgms.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jaksjppf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hnoqmtwp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pesybipu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2imgokckg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gykdjtjl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2gqfhrynu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cqxjvyyp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmkpwpkp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2vrsqrurh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ybjrkfxv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2fabgukll.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2amlhncjp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vqclijwj.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nzrnxbky.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2egdsgdda.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2awpgtfww.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2wxtypfva.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2udwespah.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2edtxrbhl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ocghxccb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rrkroylq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ttxdooyv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2sgcrqvnv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wbqxbyrg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jiketkpy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ovfcreeu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjflwptd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2plsmhndn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dgaysdkb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2yobxvbte.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2epmbqpzl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2gwblepih.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nigxmovt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lsvqzais.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2gtlcbryx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2fdkkdadc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2nlbwqaok.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kswilzzf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vywdcvou.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2egmeqxyc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2vyefqkdm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2emqjiyjy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mlnigovd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2wchbqjnw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2bgpecyna.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qppoxwqs.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2jbgngial.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dbzirmwm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2rwlpjeeu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2sixrbqiv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2onowxvjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fknqauax.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ftnpyevx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anzxqljy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2vxqwaueq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tpvvxzpo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjaxnhzc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2skitkbis.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2aaehirxa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2czglyvyh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2nplzdfub.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2uecfpxgq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lwnntjjj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2wvmywasu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ukqicibo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymlcuzjy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xwpruwmm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bszrdemd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wxnwzekd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2lrbpliwz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ygehqkoc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ffdhjdes.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lalitsnp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2mfcsjjqv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2godwcxbb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqkbpsiz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnnvjjyv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ycddewrp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cfbejlpr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2djyybnbe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2btvpxobi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dujkyiml.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2gpvfdzdi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttzfzyxj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdydudbn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bnwpjkik.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zfzopuwg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vbzqpcdz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2gbpsxdxj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2csolisiz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xhsbvklu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wxenochq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkjygzvg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zeebcfbu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pubanjjc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaytppmo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2acoiaapp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wtjckgeo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2owyscmlp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2wvzblknm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2rqzvqdqm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsgyjqew.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2iowehrtf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdgiuwma.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qmcvsnah.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2aqegkjym.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2rwsfxunf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2mgqvnnbs.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2jjvkungd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2nbxeilvk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ynoguubq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxixovlj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2snmekewu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2apvlmamn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2joqemhad.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2njuqyonr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tiwkwknf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2qeyuvfwv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2soqotpnt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fmkapdlr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mzhitbof.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qtpddzbc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2izxeynls.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2odxiaacl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2mzuaghqr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2txivrdou.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2hqvdldnv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2xfrhhanl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2poiyxmoq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dblxtgud.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqjbwwqk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qhoihfve.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cotiyaae.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ugpqbljv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueaiayeb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2wolpiiks.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lwfuaaln.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sipoglle.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ebdmupmd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mkdpajxc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rbyibgaz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2sjgkrmwi.html


<!-- 参考信息 -->