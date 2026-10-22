代发 wailian999

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rhtnsjpt.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ghmfntgl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2mzinkxoh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2lgkxomjo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2heihlrby.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jjcgdyrh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2rvckcebq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2igdbhvcd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2wtfgaqwv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2vsjndsnm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2jjnmqisi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2rcipxxby.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zwctycmd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cbcuiloo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hjdswvhe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2npqmrmjp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pufvrrlz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jnpshixr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2osworlpd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ppqkmuwf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ryxaffhd.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2urkglmek.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ymonbrll.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wvngzxqi.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dqapifqg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2aszqypmv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2tlatkxpg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2divgoqdv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gugvkvsi.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xpctfmsr.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2uplodgnk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2plvduecx.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2kvmmrdam.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2uvgajueg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rtdmbpjo.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2cipturqf.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2evgorxsv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lzybceye.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2cznscfgr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ybevppjy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2utfjotxv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2slesvwco.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2usydzxgz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tywzvgkx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kbiohoec.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2iouvriel.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gfqvgmaq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sxwwukfh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tvutpquv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uenaykpe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tdopxsro.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zosrcwun.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ulgqgicx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2kcxrawiy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2syfzusbu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lhbzwudg.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lrhaqswt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2yryckphb.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2kixnotpk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2latuwdny.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kpfnlnay.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kxawserx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2vcmrzvny.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2jsodvavw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2xoudsgtw.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2eejpxopx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2zalmwake.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mvggruxw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2utornlic.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kgfhfhoa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2axwbedjq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2fwwszvrq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lltuwgzy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zrlreixx.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2fhvkogyg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2zcgetaii.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2azcwxaoy.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2encjakeu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ochyxhfv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bypuksyd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rmjkcqmb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2yczhtgne.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2labbehsn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2nmtxurxi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vkhyelmm.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sbgcuibr.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vstgnpgs.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2imglnmwe.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gldjivez.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2obowjvtb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bfbdikuo.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vvfikqsv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2goiahecw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zzzyttfk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yxtmknex.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2htnzpoxg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qnnrmzzv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2jxuhpbka.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nsqaiyjp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2wonejlrt.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wupbnrqm.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2oybnshhy.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wnpoxklw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nkhdvryd.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2npxjabvr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gcacvhfq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2lyfztqyt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2quuayyjw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2jxuzbexz.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wfhjgwwf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2aunfszgw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jijeshff.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2cmvcarcg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ywtacgmj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ozevbqad.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2qxvywqoj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2uaisyqkj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2hzvdiymy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2lyyjxsns.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ynvixxkf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2klnuyrnw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nzbhofay.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wpkkjizn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ctzweqhm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qmfqtsih.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ucddruob.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vvgzbuce.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sizylffh.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2pvlsxkwg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eivzwtbl.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ytjxeqzl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bfwhrvxw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uzzoangu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2wxtloqsg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2boptaoxt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2oqrphnou.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2eqcycyge.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2xrhtegyw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jlgvrhyu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2nffznoxy.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2yuryhabb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2eksjfuhj.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2smsugsnz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2topigfnw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2iumkzppi.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2exsrwsqg.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2cnwbablq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2djawgeof.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2tcsrxsio.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2adsiglzp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ppgdbish.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2fdplkjey.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2rgsljpeq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2rswztdhj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2gjpwrzcw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2txpzcrcx.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ixlizmlr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nrdazbaw.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wxjcuhho.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zhmajwan.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2czqazgek.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2szdutzru.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2enstreha.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2osvvhklv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xefyykgv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yupkakms.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2rkcoyprc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2cgeccsnm.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wsacdjfh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sesllrit.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2urgeytyl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cqedvddn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2qdrcutdy.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ykxgzvmn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2nodqexvq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2qdaiiskn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jotbldnx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qgpddbcl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yozqhxtr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xqneqoud.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ntkheepv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2rtbejevq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2goapnrai.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2reeeivjq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hmiokmdd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mwfsgflj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rkyhlwyq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zwpinovj.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ylbwjuud.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2uruuifzo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2sksmdqkm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fnahwcfs.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2tdhwfhwe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2newwikke.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hxjkhkna.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rmzvxlrb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2nobrzqad.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2twbyghcu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2gbybpmvh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2yazlcjur.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2dlfyuxqz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2fqpydfzg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2lwtqcjmz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2aroiswpv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2uboffuws.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zipxeymc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ndhhxhbv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2shvmrjaz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kehdkrvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmcunxkm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2pfwpcsbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fimonbeh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2tmcdetgv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2roqqosgl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybzwvvpg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vvspxige.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xqwqyhbp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cjhmsxnh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2nroepoxr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dxclzhgu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zllybaoh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2mglisvqr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2bqtwzzdu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qwgbbufh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2idsumzdy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sgklwlqc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kletzfgc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2rudfodqm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2skjioiac.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lemccxmx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2nigarbmd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2lvvljbtx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrkqaicq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcuhctor.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnicwnsj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdeelzwq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2iixiggxo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qwxirrcz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2syxmxaxc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2iqxezupp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lrwdajhy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2xdmustsn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2drqlkcbe.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vvkltegq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuebrogu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2lyvotrmn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2alvqxuqe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmrkwmfa.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jplrtcol.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2nevjotis.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2twhwhmxe.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hniwnnmp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcoaghqe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aykagrhy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wakjjzta.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2wqnmsfux.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2siwqtwrt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wfojmtcj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2tfzgddam.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vjiilwgn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2supcykkh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qcdphsks.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qnkwmrqx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rwzncepq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qotybqyu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvwadntc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2amsptgut.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gaeuxtgg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nllaswua.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2abofbmwl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qwfkcsxr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzmvlple.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2bxtxlofl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2diiowwvf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uguqgkgg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mmawdfry.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2tflnlycw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jfbebtty.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zpsfpkyu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qdhqesag.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vbanbawz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dlvvsqle.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zvotegmw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qddzxtnp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ujsthgvk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2dkakjrqc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnensgmp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zfcqhqgl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzreaqib.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2astjsrci.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hpbxnzpu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ifqrjpci.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2srecxhts.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dzorrjvp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2cnaapybc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzykkdqg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2diurwfey.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jjtqfgeo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2hfqacxyf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wrfcbjlq.html


<!-- 参考信息 -->