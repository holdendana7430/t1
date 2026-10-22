代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2iaeqlwex.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2grjkbfqh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2hjujknoj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2shlpscmc.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qlfmsvvu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2erdbasoz.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xzrpleis.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ivscstgf.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2oviqeqcp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hpfqnxmo.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2olznmkfo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2cbarbach.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2pbdjvcws.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2dtsnrxdd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2dkbvbnvm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2hxfeihwt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2zdtugoxk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2gfodxwya.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2vondwrbn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2djhaqxpx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2tzeuxqrf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2muabiect.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ihgnpfjh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cwwxuazh.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yteweest.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nybcptnk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ooxivahj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pvnafjif.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2eoayftnq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2sdwvryme.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jkjcskhx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2edjvmkiv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rikaszgo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mqrdgkne.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2rzrppkcw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ecppwdrs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2cizjuuet.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hmvxzshz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uiyqygpn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wtpyetez.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ixzruasv.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dqfdppdl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yxehwzwy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2fussencg.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2veojvizn.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vxrzgwfr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2vjovkjyp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aeybpwxd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2svlbebhg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bbduvpzt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2jxnwdtkg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qdtmkaps.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nzodrjpg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2vhncxpii.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ufezzihq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2atwcmkgc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iypznrxp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvlqmwrl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2comglcve.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2onhhbcys.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pmotcflh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2finhhjmu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2icokztir.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjplfbry.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2oubowwnm.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2tzyiupwr.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2zjxohktb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xybmiqqq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wlxfqvib.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tpfguovp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2keqpaiuq.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2fmzlnhsz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmeghld.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ekswqupl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zlnwqdzz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qirmmsho.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qrfoivhk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wpakawzc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ubwuhiwe.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2rkizcfbo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cnyhtplx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ivtqnnep.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2gahzmshi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2dbyejpck.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2unesmgku.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2uyjzvvvn.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2odfzuwaf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dwqivkev.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2domfpuny.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2mkuqfjcq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2vzhtdsij.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2nxogkbgm.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mvfxrmnb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zqovtboh.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2khebcaqx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bnrbfkwq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hvyapyoa.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ugzrwaul.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yvulgqnq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gbfjfwbd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2pupsniog.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2rqjsgkij.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2avqntzcn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hpepruxk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vmdgoylv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2qjlmvuot.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jgbctayu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2kisbpprr.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kbgczrcy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2nuzdyvda.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2svepwhdq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dnncntxy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uzmanpdo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pxbiexxj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2eboebljm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2obujmjdn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2eymxyjwb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tpaojmkl.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2vjedbbnn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pqfvyowd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2apfwywsk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2bgpnidhx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2cdnavdgx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2capftnbl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2varwipsv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2dyfxlotd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtvcogcd.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2eofawoun.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rcjfntgu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxubwfcg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sirjclgg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2szqqdzbq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2geagkybz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nazxvapc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rrzyidkr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rexablvu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2zmvjnwvf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qqvdeepo.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bwxofupj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xssbnnuj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vdxsrfld.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ieolmcek.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2cyndtytk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rldflyym.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2qelblzws.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2bresfitj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fnnjovgn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2eiuybepl.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2oyyhxyll.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2aoikohvp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2vgnojgah.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xmmwjkgd.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ohjmpayq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2axaouohq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2fbmmpkcb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2eklmncrd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2yegkjakp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2maxlthfk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2egpjasyh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ovmyfvuw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2vjvczlwj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2nmbiikkw.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2mpybheba.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2kpinbmaw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2zshwybjj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qmtfzvtf.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rvgszauj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvfofjfo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vcscezxw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rqcpfxve.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2atxcxzme.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2grrykczk.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2myxngkhf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fsjgdsgj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2fwfswxdq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2hspkyqof.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2rulepakl.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mtewofav.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2jgqjjeqn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qnumslji.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gzxtksdu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ektnbcwy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2qrazwoxh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2gxtgncqg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yuoeboox.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xhudzufh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cvuzejag.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nxivobli.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2upxvxjye.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2dtvbidzo.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2wngebgiq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2lygrveum.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ssgfnqda.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2anjyeezl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tlrrfjlc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2cxeyjqye.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eelvjcgo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2dfqirxqb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2oavbgkab.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mxsorolh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2jbvqgiej.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2riumqdis.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2emxdwnxb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kpkpavbv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2olxltmxh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfhruygz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2unjvyunp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxggdpyj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2gnblvhuv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2nsrlzrdq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2zxuhiqjj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2zyhzegyd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2byccrcpf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tqdhacnr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2btmsnsep.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2mxjtvuwk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2oyxbqgnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzsjcleq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hbryghsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zuncxtcy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2lratvlpi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zpaiobxd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2qqdyrjmw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eufloohn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2afdlajey.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yolsuifa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2qezpsikn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tycuwpjl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ibkbbipe.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2dwkajnwe.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2bsnbyhga.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2tajcfagg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rrsflcqz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lstqeqwk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vogfocaq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2srkziffx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2acuddtvv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mwesoaeg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2lcnrgveo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2qkegiqcr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgprpuky.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sbzgqskp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iepnpchj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kuffrppp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2unzgfrwc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2cxgopwqw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hkxkiber.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ctsvvcex.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mjicbxzw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyrgtklz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlstynfr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cgzqhyqz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2wesgymgg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2abfchskl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2tinbpnzc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2krmevlhz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bluvsast.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2qmpwxhfx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2xpilihjq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmvlnthk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydefdgvs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kuqmowjm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2uxubixlf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2wlgtcius.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2bsostahp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2yjbwkecl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmomblq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2uujzktnm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xusomatl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qomnmrkm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2yjbauzqg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zxunexlf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2siafxdce.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqcrvzko.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2lgzfxeqz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rqzfdmju.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qfsrrmjj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jrxaugrp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kedlajja.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2icszfgub.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2mgwxokpk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2pxkinowg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzrovnuo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kinfsvgb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qpcttosm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ylntxndj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fecoslsl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fvganbhx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oybtsocl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nicawttv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2xamfdied.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2afzidkch.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2tkqcycti.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2dyvesrtp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fgbtgict.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2flcbddxu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lodfzyxm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ywapgxwa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fuheabzc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dbiijkdw.html


<!-- 参考信息 -->