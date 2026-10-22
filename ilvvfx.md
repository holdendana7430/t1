代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2jprtolwx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2prdyvllw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gwczywag.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yfyivnfg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sbkoqaxo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2iaqehymz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2rhknvxbk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2roaaldce.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lwfjfcvb.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2obohlhav.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2elowgobn.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jjqutlrf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ywqvrpkk.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dkwuzepx.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oehqywii.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tsrcocvk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cibpngzf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qdxmavef.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2akuaiyhi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2dsrloqdf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2zgqzzuxt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tdiwllwm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jrozjytz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2zvvktobg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2yllxelwy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2tkuaehhf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2cgaotpzi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2mlkbiadb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2xosomfvq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2khrgkvmn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zbmozizb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lxykicop.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ibrulamt.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2myajmrfv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uscjbuxd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ybvcauka.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2lwaiamvm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ezwctcik.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2swxkrwsx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hxodvgjo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2bxrahtkd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rbezrzfj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2foylfebi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2rvtcmzfr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tasefkhj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2tljgqojg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ggtgwisi.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ygfiwqec.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2trrdeulg.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bpggcbht.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2awmeioms.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2knvydxgm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2gvnzehgb.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mvwuzyjl.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2nbnmskzr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ngrqdgkw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2mqvxqbut.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2luormpln.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ygpfeyme.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2eawerokm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cfpjggfx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2xacbjnxf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2olfqlflf.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vobpqzny.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwqjuhke.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2esltfxrl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iwcjmfew.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2emljdbdm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hmranypm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2dzlcrxhw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2zjqxrxsw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hfctxlht.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2mnrqxjxk.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2bvybpzxh.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2umbnfqoz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nhlbzrsd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ulteehfr.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2aurvrudh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2iwgstedu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2fauhvzcu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ngnxiwte.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2tjnmlacm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2osxgdayl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2snmbawsy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qqlyxnsz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cqmyplty.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wkjqxvga.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ysqmqsyy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2doafocmi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2eanmhyld.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2acxjzpin.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2zzuurfav.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ywprrzzd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2doyfmexg.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2werugqht.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2qvpdlurt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pxzjjefp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2vzpnqgkx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2xhvhrpne.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2sicmwrfn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bdndlyqr.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sivnyqjk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bxppqgel.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wfqnuuaf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lhwmrfka.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jxkelhal.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fgoiekat.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pquxvlgt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2yesbopci.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zsvkmlsq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fmdiunzt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wkmmodfx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yijuglyt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2hcrywtzc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hgfycole.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2whhqehii.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yojxlzjt.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2uuqelfpt.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2khgnvibu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ibncopqe.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lpghhrwn.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rtdqyhjl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ienvhubm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2vzsfhysw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2izndzofi.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yqrijhxn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2bkmqiknr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2krioutwt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2trsgjvcm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2xsyinypp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbmdvokp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pflnahto.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2yoyglezb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2itsohzyw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2orisrmlt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2pxwiqcps.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rrefqwem.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hucmwpqs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mcqmenov.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wgiqwkxj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tdpdwnij.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kjnzfykx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nuxpabqt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qdcfsxkc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2voubxevh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hjowtmfw.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uyixoypi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2aqdkkqma.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lhriiqxx.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2mokbqymm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2mhdxzalm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2xadxwely.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2orvuffqy.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2utnnjshd.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2inxhapog.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2nbstnbli.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xgssgryy.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2acipqinl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2wafrjdon.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kkyhzzya.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mkvpleea.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2bpgvdbtg.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2coqfybrj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2xicmofqf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2hgvkoyxt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qjopyluf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2jxymdklc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2gkzymfye.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2vhnfjfrx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jgmniwbc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ryuspzzg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2qecgehch.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2olrhilnb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ftuylvbr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2csrcecfz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hxwjoilw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hlygcdvl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2aaytvcru.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2avpcrihq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2zcbjftlb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xuqpdiiw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxwoeaob.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ndvlhhfx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2dutncyrw.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fdklyamf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fuahcaav.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmrrmbni.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2sggkxgzl.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2fozcrykb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wyrimezr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hfawinqi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cjiofkel.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lescaxxw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wmnurjwh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hlnbqyzw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2lotcvgco.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ukmhbbiq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2bemvtnvn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2svnqdrfc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2xohkhjbt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjunneyy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ssezctmw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2naumxzoh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2dobvuhsn.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2eedodkuz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2bwyvndyt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2edugywiq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jbtyjdxh.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2iojbircp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yoysusum.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bzevblmn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rnchhviy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2qllfprgk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2slfsyccw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2giwsmgrq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wsyuknoa.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2acwvxpyb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2qiiituwz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2njynvpwj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2zfuffmva.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2dygwjnyz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rsndaqgy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2tpdeyfni.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ewdpuylg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qqpxchug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfcqvsrv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2njoumdmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmqgzhni.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ndaxsmgi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ltaohtqm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tupskmqr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2besexwyi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zuanuiyd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xkvwgtyk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2itifsvvr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xttpvqtm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bhazkzfh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2zrrutvms.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2uaxggxjq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2pbntwzkh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oicjrqtx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kimecxoh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jdlkbfny.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zbjplyna.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2wnvoehvt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nrvyjqoi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kcfasuhr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qijysbyi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2whyioboi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dmbrwbhd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2blkfnhtd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjfgjvfx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2lngjacsq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xhvjfato.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qjukkqow.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2oophtghs.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2htwymrnw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxezxncm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ojslzfmp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxslhhnb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkdjxgnz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2luqjthbt.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2swiujinw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bwdfuxbe.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jighojcs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2uzccamef.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lgruhpqw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2elnbnqda.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrttnsnw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpdwpkcx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2fldnoaqh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2eksdwitv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qxxhnyzr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2lumrlvvi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2pxlqxehr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbvrbebi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzdxztmw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gntyebvi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2lcuvljeq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ftdvevxd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vaqzbkru.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vozmqgme.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2pnhaftsz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ipcokyyv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2hysomtee.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeclmjhe.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ubmfuash.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2czlcgill.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qptyazvg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2owgfsgmu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kqmlfjsu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rpjbajox.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2mrpzmbwa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xszqfmaw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wrkrnwzt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pqkmotfz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vjqwlrsy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2szxixtzc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2kunynghk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sepznvpb.html


<!-- 参考信息 -->