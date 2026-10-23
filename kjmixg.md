代发 wailian999

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3qckpaoox.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hjicmdca.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3eniylexy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3hmagmbro.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3reztyluu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3lseqsaze.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3cfuymujw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3dswhflyt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3yawqjrno.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3qkihdnvd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3nmimgild.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3epthckmk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3iosbwdsm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xkxdeirw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xeuaupkg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wruvopvn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dbiefgoj.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3guqlvhcu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ejxazduj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nwboluvg.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yeafhhet.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3aclqffcx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rdxnpidf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nbziyptf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ukxpvvxt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bppetfer.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xvppxknu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3nrdazjhv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dyiebvjh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3yzmdnnao.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ogjnayqb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vvzgtasf.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3xinffwip.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3zjinofzi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sjjudpns.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3tfwsbqjj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3fnirhkse.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jblkzmpc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ocpafwad.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jjufmgom.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3tcwvdzvz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ymohdzgr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3gkpqbnpg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ijnjgffb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ycpdxbpj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3xeokwcgi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3auqfeqnw.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3draobhts.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3twbkuirb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hysjwzzx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oadyyudo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tfnouksv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tpyjdkpm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3buobugjy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3wtuymcbe.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vsxspjeq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3uwrtnfho.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3otudsufz.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3vultfnrh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3sazcgzfz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3skiztomq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wakgvwni.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3nepvlswx.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ttkamnvi.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3lxlotjnl.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3nnlckqpk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3cgaafnfn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nnhelyfa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kphfrzxw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3owtoqutu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3oaqoactz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3tikdwctw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fmvjkqth.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ylmmtuuz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3seysfqcn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3kxktdpwo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ukspkelu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3bdenckgb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3bjzlrtjt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3trqrtero.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xbldixlr.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vuzdtoor.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3fxnrakdy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3sfpzfwxp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nnwbbcay.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yemztqom.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3skeviase.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wokofuyl.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mndzbary.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ougxumos.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tgjaauis.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sczbmiqb.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ywwcwiyd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3uvnimywj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3espgbvuj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jbxkkxia.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yzjacmqb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ylxipnpv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3odixdhcc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3phfgiuaf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tdrpozgk.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xcqrbfwq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ajjykewj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bkbyzkix.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jvmnkmvj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hxsysapx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3uwhibnjh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3byacuefu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zhmpmocs.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fvklgzqg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3fnjvylxt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3tbbpfrnl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ufgxdrlx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lyruitki.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpvornfu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdmxxbvx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3fcwczcht.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3llaywuhm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xogaucqt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ecmbqckf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ifvosjiv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vjszixuv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zdbixern.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kcvzzsrb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jrplbiad.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kcanetdr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3illoycyb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iezktwno.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3pcykwiwo.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3oldufqpu.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vftnjofd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3znaknpsn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hnafhzjy.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3cdafifap.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3dnnxmfdn.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3mxqdmuav.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3avswbiry.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3mjrzxblx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3aenffcaf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3pzuauspc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vaaaxlcu.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3dyqxewpk.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3rbawgjjm.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3onmnsumu.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tkhjupqo.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3fkrnqsuj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3genazddy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3wwzdtica.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3yjvlvfuy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3hovytiuy.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dmysvkzh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3odmpufuq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3plyskpmr.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3lstcwezw.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ziyleyxb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3xnessoyk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ziifspks.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xypmttkw.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sgxhxaki.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sfbntluz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tptjcznm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3owodosqe.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fwhivflm.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3bifcbhlr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nauwbfoa.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvheewny.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3tkpstcya.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3pkejvonj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bmwsnkkz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3dubeakqz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3oxmzrbgn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zfpuxrsj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3riametnq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3flwmmibf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3tmespsxc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3yfdxanru.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3avdpivcj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hyyewinp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bybytxgj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3iakhmprg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zquxteff.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wkvjpvhm.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3xwjkcmul.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3kqdxeslz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3cmhskcmn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xbgnnmzt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wwmjiooe.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3avmkhuax.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3bpyyxiec.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3egcgpomi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tggneuuu.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mrrtfwni.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3iisuexjx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ehaloluh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozzicucb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xndqgkls.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbosrdze.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xzzywiiz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3rvvkdnjg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pauoelca.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3fjqqsdaz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3afausocn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3iunltlhz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3aprjqgft.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3mgedlzum.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xijsgysq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3rciaixge.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3juixeece.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ukgvcjcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3paitsync.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3cwezeren.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkyumptz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3kbosyaen.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3buicvoxi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhbkmcpg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mgjmmtac.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vlszmojt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3adncmjyo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3kbntwggp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3qtagkefh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zrlyvaob.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jmqejowg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3zwngvfwm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3vyrzvocr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nagjuzcu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ndnzqtoc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kqhzwvqt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ylgyyywt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3otgzhqur.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3eyuombci.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ebzsyvew.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3teksjrmz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bfxzydvy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vthlhgsp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kljtezvs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gihzvkck.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lmhfyomb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3mblqxyta.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uvveolih.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zvzchsgl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eshexnlw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ymoagfwu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xneuwsya.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbwwozwf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jobswqfq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3abujlgin.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3lscrznxx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mpdaxedw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ulphkont.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3oggkavun.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ufmjtppn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmuuvmsk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3meoysikp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3pqhiotus.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3kzckctvg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qohvylao.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3capethie.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xyphdyxp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ocrqbmcx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppbjxzdw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwhrjqpg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ixoknxkp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lniztwwq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3nsmxqtkb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3dnohjrrv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyqugldn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ismgiofu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3aqabrmlv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3neqbbjqg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhpnzcus.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mxgowrbl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nailahrx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3agnwskiy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3fpzrjnbf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pixvzgye.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3xxnthbvs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xsxjefbd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mqrtoriq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3golmldyw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nqbbotfl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qnowocfd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wfoqmfwk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3txpcotew.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bkcvvyqe.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3bgqzyqlk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ewlgddel.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3siymuixe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uinszswn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtrafwja.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlzpwtsy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hkcotkkz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3pultnmul.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwrolqez.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3cefdpcem.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3hzjltpbx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3buzncqff.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bubkmwmf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3netkqvvn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbrsmbhi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qrgzqcer.html


<!-- 参考信息 -->