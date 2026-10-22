代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tvlxurzr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dltyfpca.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yzwaqeqy.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lkwyvkwf.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2upgdozrz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kwcpzqda.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2sxfrsvql.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2mkvaeuky.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlpyjyvl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2lthweedm.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ydxcxqnc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2pkokussq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ogxeuxdf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2uvlisgif.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2brjdzcvr.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ryjzdkjo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2fawxelwn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vmhglvvh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xqnnegpn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2oqbvpihk.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ccdmrwta.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2inkzdfif.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gbfnolso.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mkgzrokb.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hvvctavu.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2orntpowp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ssxqdrhp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ilnauwao.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2krutgkat.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2soxcwcql.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2slqyeonr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2vcpdimmt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xonswtvq.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iimytdxu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2zdgoaxqt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2sviyvmvn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2owwjencq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2lhlopvwr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oafcdvrv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2zrkjoxse.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2zthkdcbr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mowfpbnn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2jskhtwtb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vgfyoqwz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2tripeqcm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ihqazljv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2jjnsiozw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rrixsocd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ximmkewb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2zhfosmmg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jdkhirof.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ceuldhky.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2evtspjek.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gprggwdy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xcrxeqqt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdqabedo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ljlfxcnk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2hhrkjfah.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2dnizjidf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ypseejvk.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2hvqvvgyb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2nrxqvjfr.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2lqkporiu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2elaezjju.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hjhhdkha.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lucpphrh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2srkotjce.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2lldtbshl.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2hvimraml.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2afopgpwf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2jlxinsra.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cfzyinuo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vzvvfjbx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2erbdenha.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yvscprqq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2bzdnncxw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gtfaqahd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rzyzaakr.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2hrayidhu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2tknktjtv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2vximtyem.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rxtmhxcf.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cokkyjue.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2mssouhgi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2aglfrnry.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hhohowdx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2lroeorhz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2gdnbkvoq.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sazukeic.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nezdhgwa.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ksfqlxho.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zamnczxw.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wnhflxrm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2byhlnuoq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2monbtxxa.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aydxplra.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2gjrtplji.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2uncfkaam.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lweffghu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ppjxonwe.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2amdgibuo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2lcejpery.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qezhldsa.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2yvfywytm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2iusokgbt.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2bettsnkk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2afxskibz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kfyjvyow.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tqavoqnx.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qaszxemi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ppcyewwi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2lqnpzkfb.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jjagyyor.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nmwdgfpe.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2pjrindik.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2mrlwnyrs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2emlklozx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ejzqtnio.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2unpqjurq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2vflwtsec.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2bbammspp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2dwgaajzf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2obrgsvqg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2rvggtjjo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cvgbpncm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2emvuhbka.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2udeusiqd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sdnqcghu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tlcjjtfz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ebpyeddl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hfphdmqj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cfctxjrf.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2jlbgvpoe.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2btvmkkuf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2sucushyj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mblxqpbb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2idouiupq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2npdwuhnh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ztbgsyyu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2hqmodvmy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2wqqwxrvq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2exhxucod.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wwwbiwen.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2mpzzqhvk.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rsbtesia.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kgfkuxwq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2vvmcaolg.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kalotckb.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fdoaynar.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ciieciay.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2deyefyyn.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2kondfafz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ngrypwyz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qfompacc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ayffvpnt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2smetbjry.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2bjjcuuhf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2xzbpsdqm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2unehxwkq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2skzneanm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2wyteiref.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2toyoamsr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2elkzkgyj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybzktqlu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uujujygd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qfaqgqyg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tddwvacx.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ayouzfkx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rneatxsk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2jxmdviax.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2jwafakcz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2uwhphpbw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2aagemodx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2bunwgosd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwqofxxn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ytptgvje.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2opwjuzht.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hcjisbtq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2hmckimho.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xhezlfic.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lywxbgtp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uzmjuuti.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2txazvanm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2nsrgkkzz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vlaatbuo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2svocdwzx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2srujatjk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2hmppxtbd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2pkkdqtmu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vlcxxlgg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ziedenom.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2czmnenpi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2eeezuqhk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2rqryvwsc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pbqhmzwf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bueifhdj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2abxwokej.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2vsfeaewv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hcubdydi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2evlockou.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ctpdtkbe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nsfgtanc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2xtxcmlkj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gsvtzqzv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2zazilrtl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2pghjljbt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xkosacsn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2mjbeeuth.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2swrehlwd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tihpgncs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2skuryeeu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2wrevtnze.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tykmvfsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whwcfngx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2dwcjpnxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwwomdoz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2dehpihrk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2hnprdbxj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2udgrhwai.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2covvbbch.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wpaxgiva.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mivnknbo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2crhauaht.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ooqycafz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lhkleqay.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2rbqekypa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2telacoph.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qivpqvdw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2umolmkhv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2binskebq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vxacbvzy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2hwxpwkpf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xlvfzqzb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ttmhajrr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bbijelwc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tjmlzjwg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbeqwnow.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsxrzswr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvvkxoqt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iunefxao.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2aqsdebzd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2yvrnnspp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xwvyoerq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qbocwwcv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2uflhrapc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2yucxdbbi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2szgviffj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2soehybiw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2gnndsppr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2bxbbfmve.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2uwnkpsiv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljaotsjz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2whrrnoeo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zvecphhp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmhdiezb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydgpoxhk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2sfihayxm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2njjmyouk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2upuxnnzf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hijaslko.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2cvhjrgvr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2poewlqlo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qvikkqem.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjbzqbeo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxfvwosb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzbrhhnp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2iqxjnigh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2sxquujns.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2iutnxdst.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pksyotfo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ywuwkjyk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zonxlnxf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pjrkmtyh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kelxhamp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugemecwh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekrrmalb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wliviwqi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bstcrvah.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eogfcics.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2jiyvlfsu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wjpabwgd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ndkuhhkm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2prwlglet.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2shouyssk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2esafgzah.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uyhaanxw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vpfhboso.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pjfshoqn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2vhjlgukl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2mivqpmwb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttjqimin.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cbwkuhlc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ybknklgr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cegdenun.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2teocmcmg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xmsvlpoy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dexnvpik.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gjgxzpna.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ybzjktnw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kakjizdm.html


<!-- 参考信息 -->