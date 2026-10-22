代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yxzjillc.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wlolfjwd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ppkqkdbh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kwdcqpnm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mciuoxsq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ootryfkq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2yqjruiih.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2kmzivacw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jadepjxa.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2nqeluuxn.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nnredrvj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2rvvetchc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2zanhhfpj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2grrpviuh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2rbrhamvu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2dchdfcgv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2pojawgvh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lhpkpfbh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zteofjwk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hvnshegm.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fkvxwzbg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eajzgrcn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uuccrogj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uzefhyfs.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kverehsd.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fnbcevny.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2olbrmhtd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fpwsrioj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2iiupmcnw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hposgtke.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2bupawtnl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2hgvvqkvr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zgqptzke.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2juqzczsd.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ryxcxhte.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2xrvqfcpt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ndjbrvat.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gkuugurm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2rqctmvjf.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2dxhnnmsl.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2snviewlt.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2epmsegcb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2kcwfdiym.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2irvdujgx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihunxqzq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2whjzeezy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ovshepho.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sywzlndj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cthlnmpx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2hkwvyagt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2buanesyc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xhgsorhm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gjzqpwqz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2duycihki.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2agxscdik.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dygqudck.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lntxzczw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2fehuyafq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2mgbfxbss.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xcknkaev.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jvlvezfr.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2volwouod.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2feumebrp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtsvjtoa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vcmzfvbx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2paxkryhu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2inzuomxn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2vrscppnr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ntbivtdh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2klhtfpkt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2bvfnwtuv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2exhrybej.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jmkikmyb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sxefjlih.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xrpjfise.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2faazkpon.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fulhnhnf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mkuagqgo.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hbuzdqsk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2pxrxelnf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2rqttmfjy.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2xmmksjeq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2tulrovaw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2dqkfhxtr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jfrmtqfy.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2usfxqwzx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2mmdasegm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2rvyxovvn.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fyksagrs.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ipixeqvq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nctlaahh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2euirnrln.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wzmhkfks.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pqxlpqkd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2anoityzu.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tlrbpftf.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2bkandfew.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2bkvkxqew.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ogkwyufa.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xcsubfnz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ftxkkpyv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2zjeajckk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tcxgsowd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2fenlmpro.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xwfrxedt.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2keuekriz.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kpshgtka.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fwwtrbfc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2neagqjld.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ypbxzekw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xymniwcj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2rpiypdbi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2awzuvivp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xiwykvvf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qmwffgrc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2aoislymo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2pysvorya.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2vmwcxwxa.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2pjigbvxf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrnqbnxj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2wmqczepi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2obzpyckw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztqljxdi.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2raopelsb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zvakslmy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kpkcwiap.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xxsqwbuv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ymcrmruz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ihbvfqna.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rxalvuoi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uijbvbww.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fdhzlhbx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ruzajldr.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ppuzkeuv.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2iscjqbsh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2okkaxivq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gcnonlvp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2noabbwfk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2mdtbguqu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ifcerdri.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2hlkwqzpo.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2gtoobtwx.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2cjqrxkdl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2oluahdfo.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qkhvemha.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qjnfioyh.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2kpsiyxbc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kzczsuwi.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ybkjlwxb.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2gvqcvbvl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2pwemquhc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2rtienvkn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2vanglhnc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2iwntapjg.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2bbkyppvi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2bvqkeuqp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2binrxdwq.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ohurleru.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2wcfxycgl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2jckatzqe.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2cobtweud.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nhczscpb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jowqwmvg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ddgsahni.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zonxfkeo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zzrrjkoc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jhbgmauv.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2bvywtvxn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2umidttvv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hvszlmqk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qkbeixia.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2zufrqwdi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ujdrsobf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yvjjpdld.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2voakovrk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dxnkmpew.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2totheiuu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2aclwuigy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2auvvblop.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lgdfmaoi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2enlutskh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zwfxmfzy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mumoffyx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kwwyxzmd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kwjglknd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2aiawgfpw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2hptyyyci.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2jfxuixag.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vuqmwxpm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fnqoftyh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ofduvars.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2kcrlpgaa.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2lwotlwhy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2yyunhrfl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2slcgkytr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ohhpekci.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2wkbgswfg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2pplqehig.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wqaeaeix.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2twgpdacf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jytouoal.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgajrbey.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fjjaqfrb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2msrbkbmo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2vxtwraly.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2vrdswadv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ctqkrhyv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2sqbaetws.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2yiizymik.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ogiwwhqg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2mlhmqltd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zrorepdr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2agnqonku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpvbyalp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2zgbjvnbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqmipfmp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2nnfbfjou.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ztjrlinc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2qrroxqkk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mjmfuaem.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nzliveco.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lbjfrdks.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2helfjwnf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2diarwguf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mijzwgvk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2znkqcaiq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2aqvopcjy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eesxspnr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zhccboit.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pbbexnuk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ekkpwzgi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2fvosbbjz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2nvdtgtmp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qqbfiatn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2roaofpmr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jbjkxxll.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2grgbtfld.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zfncyyhr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bapkrawf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2awaqnbut.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qbmspyxg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2frqfhbpk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vuxurzvs.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qksznzmo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ozrpbjqv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2aimrwabc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugkwmoef.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ktwxszdl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvvapydg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2cuambkao.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2etphhicb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxdtnhyk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fghvaapg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2lvbjyscl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2mniljcrb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqpgqzye.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmvwlnxr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2advnivew.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2vzzqcrfb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2joxhmcxa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfnhavhc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2xiiaeoqx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xyaatdho.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyruckjo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rfrblpgq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgcuelxb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2iqehwvun.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2laluynsq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hjcpukbj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2fqrxzbqg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2jmpcndfr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cumwbccp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zbelfhuf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rethgseb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ufhbfyoq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjybcrco.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2cdxttmdl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bkssrcjc.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2grsjaczm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2crungxrv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wnogzxxf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dkmvgbpr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ehxrqxed.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2inbkrpyo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lffsijoj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2byqaxdet.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2moxawgmw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oqgdwpab.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2tkjhepvu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gvcxpnwx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cptmammm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kjqavdpm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dxooczfz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pqcgfhwj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dmjwendb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qecbycvk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2axfytago.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2oqaaawaz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2mbpvxofi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2qwrjpgos.html


<!-- 参考信息 -->