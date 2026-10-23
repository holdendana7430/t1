代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3exawklqb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wqfnfobx.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3isawtqmm.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3njwtnftm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3buycfpcx.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3izbhyhki.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jkmudnxz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3juncrvzs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxbxgwnt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3syssulhe.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fmcfixoq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3bgogylat.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ydjrkrrf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3rkwiwewu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3pwtknpag.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3fccjhnyj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3oobxlrca.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3enewunin.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hasglsgn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3enmijmcp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3efuzxbsj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mhzglnxx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3elnhwuas.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3essgvsam.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zzeyfuwa.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yvpbowrk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3qxvuhijr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lifmrooe.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zvvqxtul.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jhrrgdqk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3lnvavlgz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3hlakyzmu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ymjsqult.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3haktwzzu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3pfxjhtqr.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3geqitjbz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gxrqgkgn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kaoazqtd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgefrai.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3zunevjpb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3kisxcgjx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3kucllnzf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3nztkjpfp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bysbtlok.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3yrpmpvcp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bkrwphsz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3iqjtgtir.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qltvilcf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rragrqbo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ejzcjwta.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vmzrlvnp.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bbrosmki.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vvmqjkdr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dkckgjbr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qripypyu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cptbgivv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3agfwekxu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3brisucgc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3urijcycd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dzsqwskt.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ggucwbzu.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3qosmmllg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3nvevuerw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3aznozeup.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yhckkqyp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ubehcegk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3chfxcykz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3hwwlyosb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3mkpjlrcs.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3klrsulsr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ekjjrafu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xpzismdq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3miklxwft.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mntvaptf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ohswwyre.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3rwafovzh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3enptvbqt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jmdktakg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qsvrtvjr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3popxoirw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ppazfuve.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vtaeoulp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3roboissy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xgxigzjg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3axhqtzjm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3prjkwrhe.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3dyppqvxa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3epkujeyp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iuosdkbb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sjedxsdn.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cdomznaa.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ysaxbfvi.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fvwsyvpv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yoviodqb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jtiowrav.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3glisvcus.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3adhoftrn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3qawzyjbr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yukbygsc.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bxmoiilv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kymtpnbi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3yaxofwdn.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jqmduumc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3jcpxjqwi.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3sjvprgez.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3dnegrlkk.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mnncvrjp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nwkqznyu.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bzqoqakl.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wpavzirb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3qxqojeqh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3opfocyij.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3aczisejc.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gmrukjod.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3juupxdqx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3yutzohbt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3eycerpfe.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lgzeutuo.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3epwewdcu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbbhjljb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3hcgsgqtt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3tourczyf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scjrgwuw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3xnnxtshb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3skylyuzn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mmqsuccr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nnvnkbur.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uueqlugt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3prezhrhz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cgigxpzw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ztckkozk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3biolukuf.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3nmurtvou.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kxexipad.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xhpebult.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bxmscjyv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3aqxcsrac.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3wijxidps.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3brzcpckd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3pyrgimfh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3yvqxcupd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3gcznrxyl.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3utltzmmw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3reepfsqd.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ryjbmdww.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3tkpchlyj.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3nmpchgyu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gvfzhbfv.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uyuuxwlm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3afwfelkg.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3npwfrfnf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3uyjkaehe.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3kugtegxv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3gweufcij.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ytmgrbra.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3xwbkboyo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3hwihimgm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3newyrdrg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3gtjnvzht.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3pzpbigbu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3kupqnhyg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3polgwlki.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ljfrgilv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulzctcik.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nrmotemw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ulyfaplq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qulbhhoj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3pimllqji.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wnffqhho.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zyqrxnot.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dqgspdbc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3makrhpfq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jnkuhopx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3jsezylxg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3vudidawz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fpxafeco.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3jgbrrxvl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kuhgktgn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ampxxfzd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzxyxhzb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3srecnoaq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rzuujedf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jhgvszlr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3klwciqji.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3voendbuy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3kxmydloa.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ylczutki.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3yfhktqib.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rogzcqri.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jwbayyia.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gxfefyeu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3hzjjklea.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3vujbkvwg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3dsckbaxy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yzwerzaz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3alryghzl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3tcyelqzp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ureunxdj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lrrolvyx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3afiyqhvh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gmswttzz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebxisxmq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3lqwzhfbq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxkmqzqc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3gyhtaykd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3qqqfjybd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3htqryifd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3qzsgskbv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3lkppssdg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gnzhdtkw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3qbxtrygv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ltbibujk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3miadhesz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzghnhvl.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3bslxjcqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjhzxnic.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3bbslrylk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ntoaqfqn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3rxwluhgt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3blkkrnbd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3aohyufky.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hgpoljun.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3bohxedzp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3sppifias.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rstttiun.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3eubhjcoj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3zqqnbxxe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3gmwzunmn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3teifnfqi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cpkrmmen.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pdlfwcbk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3lvhjjjbf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3htopahvo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3skrtokih.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3hjnfdosl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hkodvwwq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ydeosntk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3atenynqs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ervtfkbh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogjgdelx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dbdkrfrn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3tzuvtehx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3eksqqoia.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ffnuaijy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oixckbqr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3paulozbw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppytrmhe.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqqscgls.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wuzzafxc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ixdtklwq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3bmmseejr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3atnlrdti.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bxjlljfs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3oohnxvkl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xghznenf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3emtqgufa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3svwkcdtp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhozyqos.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3eaydyudk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3wbybjzes.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3srtvjvsz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jvhxhvxg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3zqoqmlsx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3washstyr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzhjicbj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltqjglsd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhnfmogq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3fyglgodz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mugccxsy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lboswxny.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nvxajnrb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3iwmkufdv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3uwbnkxzp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nxcdzcln.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gmzuulic.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lufvxjit.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3viiyzgbt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3icqjgqoy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xxaospdb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cojysnjb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mbaoyfcj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3esddnzil.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uwkwspsk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xxwhsstj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pifeeuzx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xoqoyrts.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ugupddos.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3omwgihpy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3nogifjqi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3pfcafuqg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3djobgyzp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ggwbnuaf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mpxmdgsm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3awachrjv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tcimcvzp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3syujnyby.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ulnullre.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3rndaeyvw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3rjimpqej.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3jmsdzzjb.html


<!-- 参考信息 -->