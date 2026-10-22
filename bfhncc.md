代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qjchadmw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ukhiyclw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2cjjeuaig.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2kxvnpqsy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2kvwcxcwc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2tcnnotbg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2uinzqbzh.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2stdtgwlr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2kdcghtfg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cyubplgb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2otxvoyzv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lqffdsja.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dxxfisdb.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wjjwusdo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zbodugza.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pegusfeg.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2gwwmetyp.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2esywdhnm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ggyrshyk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2nwqkgdol.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ozrmclmy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2geeneyhr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2mufkvkjj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2bboxcmki.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2txjerjey.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2nopbyrfd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2seyeodvc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bxddlwyp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2rtrvjpfz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yocrkopa.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xnqvgefj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ofvjxudg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2aujtzark.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yfxjlssp.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2khkpzwlg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vqhpfcrq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2xswbfxjn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zdeobluh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2wudrleaz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hopdnuoa.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pjnltybr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2rsyypprt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ogmhvoup.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bjxecnpc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bpyhjzzv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jviwysqu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mjqkcxmj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2acwkrxgx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ztarsdhi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ouflmgep.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ybtxlepd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkkwlgbl.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zjiyxqcb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2kybsrhxq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2cppdtzpd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2brjoptag.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hdjtrjdu.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2phfibmur.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2nxdofuhm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2xshxvnwx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2jaeuldbf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2zhixzikw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2orzgvxws.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gckhuzos.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2biwxotzv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uolnmjgv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kbemdbmf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2tmpnzimx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2livrptdx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hvkinzms.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vtoonbsp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2pgqsrqhz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2qxjsyizr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2slukcqfj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2nxannmjd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hxtdwjyb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2nmfoiggm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2zfgjdxeb.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2pbqksugp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2szkyjxet.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jmtbvfwx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ofyiihev.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rjimaguu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tnfqosfl.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oczjdjmc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dlxiuhzm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2punlfclg.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yduolhgb.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2hkyyauoa.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2nnlefivp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ljfkizht.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qnqhcuka.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2abayglaf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2knnrevsp.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2izzurljf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2suorzdfx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uvgrhymp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2sbkaxpbq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2shsnewiw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2arawhxax.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nitmdsrt.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sruyfynh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2faryfjhh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2gwlfzhuw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wozmkfvs.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xfjoagpj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ppmsumqw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2htfvoecq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2wwthasqf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rbydeubi.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgyxmvdb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzupyyke.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2zpxlrhhd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rzxeznxt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vikpwcdq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2zjyzihfc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kyckqvbn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xnjlcabh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bmwdwcfb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zycxnqve.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uqzijnfz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xmnsuppb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kjoftivz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uzlymbnl.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2fptweqvi.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gfuialew.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2rudgkxpc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uayfkpgt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qqlglfri.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2rnnavhat.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ultgdiwi.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2xyvgmggq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2wqzeevaj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2qzynkanm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nialqvfo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2eafcbgwt.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ahifbugq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2sdhusnqf.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2wwxymsxb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2azzxyhwj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2orrsyiuh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2nkxyneih.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2yqmairtd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2xvhtmcqo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2uqstnjsm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2chweczpa.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2itupoouw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2zzgwsavi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2budnowuu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2mtsnlewa.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2bppteyta.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2tijgefid.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2wllnsoky.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2niuahcyn.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aiakxcfn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2egqcssjr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gckgazge.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bgzjinod.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dbhyssnx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2xlwoqnvy.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iphpuuvz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2hfdzzplq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2deqdwmtk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2vazwtdgg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2akgyloem.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hmbsvjym.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dpsesfok.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2iowpyvpt.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zuuzlkcl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rtvtkenl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2dqqbugeb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qoebwipb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fzzhukze.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gpvhjemy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2stnjykuh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjlsdgwo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2eyatyszq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2qxasjtbk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nutlwkoy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ouhnffig.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbucmunw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2npluysgk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wkhxtqac.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2nilyuysq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2wlqglbff.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2yxhssdii.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gltatoae.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jhjvczco.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2bfpcjbdk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jphovvik.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kbvmfmuc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tdvlehsq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2nyrexold.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lvztrkxf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2szicqcgv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxkbolcy.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tbbaemwb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2nguremqk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2urhlldau.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2xbnesmnv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2dzlwbaqs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vkkxpufx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ffbqemif.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tipzrjmv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xmfsylvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqtdpchx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2mlnmboyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yquoriqr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2fsmrmmqg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jnfaucyx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djlevfmy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vuaojias.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2flestthk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2avtnthbe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2gexzrein.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ylwwflum.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ignqshor.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2jipxkbux.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ckhykios.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2izfkeofz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ckihwvpd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ucjcnbfq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rqztyzmk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2sxhtbraf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gxeemjbb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2eiwcgptr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hrotavzr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2sntlwoyz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qejgpxnx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lginvcly.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nhkdbsbb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwupvkfs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xdupsobb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dkqrwubo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2aklgkqme.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2thijuwru.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2tbqwgtck.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2idvihgoz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfpukszk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mawsbirf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwikkqem.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2vmxuzpns.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2vrilvqhs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvqyfdlo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2twzhnlms.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xdzsgwqc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfuestvy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjvpemzm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mlllndfp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2szwrmmkg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wohubuit.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2btmrtgqk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2teexttai.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2widccrpb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2gxzojhaj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkcrfxmg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncwjjynh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2eniukmxh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dspyqvyb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2pjodhjkd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vdhuwbrb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2aytstezl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vyjgknub.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cnqunqnj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcljshnt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pgiiuxix.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucvzwftn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxbjnevv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2nnhgfwll.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2yfmwlrjv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsgcgeby.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2btyfgrls.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2lkmdefwr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2abkmnhhp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bfmeugii.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eqydyocq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wadcolgh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2yqnrqunv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2kfddlpri.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nqdtbzaq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2vmpocvop.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2zfjvhapb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwngappa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jazvbwfg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bwygqylc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mghdnbyf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xlrtecnm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2sqlypqwh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxapujzz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2vejtkzob.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2vwrziliy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ezalaqrp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2aejnqdsd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qzwxgozg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zlqyljyu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2meyttccl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fvhstgit.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ntbzqahm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2qjhiloyp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2uedomnsd.html


<!-- 参考信息 -->