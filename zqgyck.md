代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jwdyjxow.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3jiwffzbd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3vuhdghsl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vbbxzuqp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hnmaavpz.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bhfzbghl.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uanojnuw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3gtavmwvk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ssydacba.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bhdrtmnk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3hxybpqgp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3uqexbfzk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3hwojuadc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3baqlmjnr.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3znxgldnj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3niujnely.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3xscutyxw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3cyiytult.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3eeozkxly.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3gciflcfl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3masmogkd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lunzazoj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qrbrvxlh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3padxqwbn.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sucfiyni.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uevhznnh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rujnuptd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bgcnizlp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xdvaoqeu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vnbbweaq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3tccierzd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3camkgpxu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ewfijgao.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dirmiiop.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3wyzcmyop.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3mavtryko.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ifkyayhu.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ochmxtwl.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3nqphgpek.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3iemzplrz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3natfyjzg.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vcfedhso.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3mvvttkxn.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3eyqbfahf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3rrxjahlf.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3orqeqmqp.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3fhrpquth.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kgyxnfoy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3fhzpximz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tejgppuv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3jqofitkq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3czlbiyen.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ddpjximc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3lobzuutf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cthedjep.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rqeyueeb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aepedlab.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3huftbnzh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3emfhbqyn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oohsdpdg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mltfzhhr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3wrcdgzhz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3hrvbnror.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dnxrlali.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ofbikcgy.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3chhwzjxu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3jkkjxrzm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3htgzbsak.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wyaxptnu.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hjxedvmn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3qbtammjc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qxgesnwf.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3kaguidsc.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3desgajsq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fzkmnfyx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3edyxyqfv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sijpqwla.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mjdlzhuv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jqheyekv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3mgddwaha.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uxhcchpa.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jdmsuolb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dtglxdxx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3kzlwncxk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3bkoiqleg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vapahztj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3odwiccxf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rjgjpred.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3jkyejptv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ovamyrmz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3uscxbsyu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3uingwrbv.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3piaakicz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mdtupwjs.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kgksxiwh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vlcbgvku.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cfeavqqp.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nrwphokf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hbbuhcpw.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hevtvqmf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3quzsmcoh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3urnuhzie.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3smykxoee.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3weydnuca.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nqxzbtgh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3mocfekai.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rxqweuom.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3izdawjoc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mohonhjp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gnesdeig.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xggglqfp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cnysmsqm.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wtaxdgui.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fecxhekf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3qdjwxbfq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3vvawrrir.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zdpnxlhw.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3okwftqpn.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3ioqojfaw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3efxdqmlm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rdvgxvxr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3cfdemnho.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3psfgtztw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ufdqnteh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3xqjygisp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kbhbihxi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfpibijm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3wjgirmbq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lweojlsz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uvlwcwbt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zhkjahwm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lukotmni.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sbgqzgsd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sklxoyie.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kptkzzce.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wforlsku.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3dhbxxfuo.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zdgxqrhr.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lcvbhpce.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qkirhvpu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3phrmooie.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3pidhixpd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3qrkniidd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3bhcpzkvy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3punfdook.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3moanlvhd.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jrvvuafb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3gdlofojl.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xwsvxins.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3badhguwy.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3kzotpxwj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zkxgykmu.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mvyikyud.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3xqvhqkzo.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3zrajporx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3xbolrprv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ojbbptko.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ctllrzka.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3emyojhko.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3hlfyhpcc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3vbrbmhxt.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3dshvbnmz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3bddwdodv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3bjahaxua.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ueakqvhk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yxqpiptc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pfmnlsam.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pirsczje.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rhiwopzi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fzlcqqpy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qgufhfbe.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3qtrfuigq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3aqazjbht.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jgrgwbfb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3odwighlg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3sngasgwd.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3zlgqzqcz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mdmjrsyc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3lmhggsui.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nkoxbyoy.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nvwayhgz.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lmxlpkck.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3djlylcfv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3epldixxh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3oaosvkbe.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kgxwcweq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3avmmnpap.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3olxzulwo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jvbnwegi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3lscdoyoi.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3evkqmzmy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ivmnastv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajffvloi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3awqltvbe.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3abefnolq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3mdbxlabb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3osuuqtnn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3vciutkzz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lfwglubu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lnnlpwhx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3rifizkhg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3baxpvmml.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3izabvarf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uiayttgv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfplgadw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hraxtsvo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3zbojtalj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rxkkpleq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3vgoaqnyb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3sxikdgyy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wmwpxtid.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qwrkazrg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3uoggfkzc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3muwwbzzw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xixrefeg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3hxhqmfip.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dylwuncp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eozljpdn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ihpqoqvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3noaecgbe.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3zldcxcuh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3tiudvlmu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3hsbjvlkn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3iatxhtjp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3faoyuvgn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yeusntrf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hphwwvdj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3tutggmsl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dvgbqflb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ptctjdvq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3likuellq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqwbqnlz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rdbxsvxs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gayqlzvh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vdfttann.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3gwsuycxw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3pdutbros.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sojzdlxv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3fkvexapl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bfyhwbnx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybbwhafv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xuegdjww.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3etczfjof.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3samdgqvb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xjizuyzx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3volgkxcd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gyiemlaj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3aytdonzw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hlmgpbxg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdwnqphu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oewrqome.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vsoktwgb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjqmdehm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ebbhopzs.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3sqppgezo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwvfcsle.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sbypldkx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bxwstntz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qglhjbmq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3yzrgozru.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xkiewqjy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3gqsrrbdd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3dvlrzogi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3gbshdanj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3pzcbubzx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3hlnfbzub.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ungmofbt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iojxxubz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmlcpzyu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tojifvdb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jbscqkfg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3yicqbjhs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dyjbylxz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqrptcuo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3jynbvzmk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3pcfrsooi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3oqkdsjso.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ljqmcnrs.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lqfpswfk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wkgxvwua.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3guzkrsfx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3mgwuwxqe.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tnjdtyld.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3dmntdfvn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3sgajpovj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vkyhjjoa.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lufzrtqm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3afoofmex.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xzdpxtjl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3oafkodgm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kginirqd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vsdktvaf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3xrfeosbi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3hvjpebbp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3twejsrzl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cheyckny.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lcyytzjc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wqipjafv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3optqwumq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ppqtcbsy.html


<!-- 参考信息 -->