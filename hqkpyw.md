代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yhcohfsk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2txhozacf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kxbebenq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2wivxachc.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2wpssfnnq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qcmshikk.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vmjhfqpb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2yzropryi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2kigfhlod.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2udndkrwz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2mnjeenki.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ryklykkl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2bpjhwhbg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2aidkundc.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2mzjbfczu.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2fadbxctx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2pcowwkur.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wwpbukuf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fjtbrurr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ztlpyaco.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2atzykyis.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fkojlehc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dhobpved.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ysxwamjc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hifafszi.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2eqapedps.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2opnwnwes.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nokutcwy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vorjzzkz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mfdsvtjc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2hxikwvqf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2glcjkovq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2oigjkmue.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2pdtrgkem.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2pzglnihd.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2uvjsuguo.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2onexzfen.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cosdfjru.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2yvgwxyfy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tdohxlou.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2hztrwixk.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jmvyhlyi.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2lxcvmbrf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2twyaklws.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2nbmapuge.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kyiauham.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ojrcxyln.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qwvgqiqi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uxhnbodp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2jbrvwkas.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uikyajfw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uzhtiose.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2afeaoywx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xpzsmkvc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mbzfvbor.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmyshkti.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hjvshzkk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2xevphakq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2msssiusx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tzstdjta.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2eopzkhum.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2fatdvrxi.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2wwholoou.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mfnaqilv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tjucqssz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vbdpsvem.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2urwatvcn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2wruoohlh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2xpdcohao.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2szipgdbw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oysyydkc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vlazcfjj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vrftrqqk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ttdooihm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wqzoktpm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2zvcxbkbf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gjnivpho.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hldxwsef.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2icsruayt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2flixsasb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2parnyjth.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rgnpbwjl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2mgzzwqme.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2vesvsbfv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2qldsyouj.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2skwczxmu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2egivepfi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2sfgyojao.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eboekpgs.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ahkiyzpw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2foigrijo.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nxfihnrd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tavwuncc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ykmldije.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ktairlrv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wjfglihw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2clynitwd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ivghgvys.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wmxncamn.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wburwlci.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nbivlrbc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2fjzuxezc.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lykwcnjf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2zvbagtxg.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2febrkuxd.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2zccnlvzm.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ehcmyiqx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zkafwldx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mwwglakc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mdvdgwej.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2srgqvksz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2pfqgmlfg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nyeosjwk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sdkjqrek.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2htgadyoz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fuhyfbip.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2clcxersu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2hvhwtnye.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ytwqaadu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpclrerm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2rqslmwag.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2elcyzwva.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfqgqded.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2usczjiru.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2phehwwov.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pxhdtwyv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mjjihymi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ehncembx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wndhwdyv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qnnkuclo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tupoxmht.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fnfsmojf.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2iqvfwcjz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wmjhhhbu.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nnsbbitz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qndrjdas.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zdvlodyh.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ghlljiil.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2rkzkxrmc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2lnuczgjh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2bqfgmsdc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ofplninj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2cfumibrw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2qyxjzmue.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2itsxafjl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2pgxivwpq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2pyixxvlq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jkubofrt.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kfqidqzn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ellzyray.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2wtadcjpp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2xzhnbuqm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2kfutxptv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2isoadapv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2mqbwaabs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2giupzkvv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2yognrprb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2arjarmfc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2vhirixcc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2spoqtcja.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2lbclpirr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2reyddutk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vhzexusd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dlvacxha.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uymtcfmk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dispizsr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vupadnzo.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2onhnyfbx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xacxpttn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2shazlhra.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ahvxnywh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2khhppbre.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hyiaawhx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wrbtyfwx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2wkezziwt.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2omaudhbc.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rgxzbrog.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xjsjmyuj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2bbzergwz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2vxrmudiq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kaxtxmxl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sztfhoxy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jdjimnfi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2kotcyzbb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2txfwyqry.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dqkkljwy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nfnobbyl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2tiginwnz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2dfyhrvjj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vszmwpdg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gippxymo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ignbgkft.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2mkcttxid.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2yxgjetxg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2azrpizbj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iqcoutki.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ixdcjrrs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eluxjcjt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lhqwdypg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxiqjlcx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2eugoeslz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2eepfizwv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fzktwnkk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wlhfleyi.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2wopjlwut.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2jtwtqedl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2fiabjrzy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2hcpsjnfk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2zmtotoaz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wqtkgput.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jwjkkwok.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bhcvkiiq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2iuzsnbwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jpdnavya.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2pbsgtggi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btkmicmg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2looemacc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2rmrxaent.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2qoiahybp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ufyzosul.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xhrmlicb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kllvwpgz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2kkahvhet.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tixjkavh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2juqcdovg.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2nrodfkqh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ymwlcpzs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dejtcxgt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2affdhezj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hrmvuvhg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bkjqblmr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2lkgkaxkj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2rviyvowg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2itrmagqi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2mwpykipi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2dnzvwjax.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2reaomumi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsxiojlz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wyjfldlh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrvejwin.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ybsiifmv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2oggppciy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zysxbwcr.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mikjwbgr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wadupjcj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsshmlea.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rhejspyd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2txcwoylr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2aneifnwa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ijdwxpzw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2tyoauhhg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyxyfaug.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zccknxcb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2jpgknyjj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiyzrsji.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2syblbfjo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2iqfwzlqm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2evlwwbbs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dcfwizsd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2nsrwnntp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2acbemwki.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2xpojbkma.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2mhcnjova.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imviwcyz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftmbmsur.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzrnxtsh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2oqvdzsjj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2xkxfbtvo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2iduiende.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxbkhsrj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2bjkkhswh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2twbnzede.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezbufigu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2khzcynkd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xatxwbqw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cgkpqduc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2zioktlke.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xepkrhbt.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdvekkoz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2uxdcncpw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zqpivguh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ssbjtchw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xygfqdin.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ckftmcgq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bcntfmuz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sexqirkz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2alwcevgk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2koadapif.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2kwjilfxl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2vfwylpdi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gakehobb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqobfcrl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2inrxlwwd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwzkuhcx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2buxtarqf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tbuqqtqx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xuzmgafv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2tbottvbf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fyyodkbv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2juzctobx.html


<!-- 参考信息 -->