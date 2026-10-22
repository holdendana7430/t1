代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bqqwnvhr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2byzjnavn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2oluuyssn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2kqwsnimo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gclipkts.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lzmdkkxx.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lknvzmop.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2eeradrlp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2jswlsgru.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2krddbcbw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2yvalqbca.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2xfsiebxi.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2eacipvrh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2zchvjdlc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2demhszju.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pjhqmqih.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2lnstglme.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ragzxbgu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2bkqqegqz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cigodwlt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2evqkfggz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2tvrrtoxr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gztblbsz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qxcxxewn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewecerxg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewgzstuj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2znewbgiu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmnpibec.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qghjanqv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2rjgwasol.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2mmdsmstc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lclwtocz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gmvfsmqg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2xntakkee.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2lrutbxsu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2bektwzwh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mivwkmen.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ssliampw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2fgoohbkg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ctdzdjqh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2eycvbmus.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ynrkasht.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ykfpslav.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lqrlmtas.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2flyvrlux.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bdrwjcoc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2unoaklzv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ehmkrrch.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2betmxbvz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lwfeejps.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yuoxtyyx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2fbbdjhoj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2vtkifcyd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2toynclyn.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2sinihldn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2tfleixhg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ljmprybp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ofscrlik.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2vixgogge.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2sscowpdg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nyfdxiaw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qzlowksm.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gfzycnlm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iaqhnztd.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xidyrqlv.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bjrnmupk.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qpfndasw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pdjqbryz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2iddssedn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2rcykgdut.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2htwzkzfw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qjajwdrq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qpwwwgqk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ovlaqzdj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rdgrjicw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2kmnjfsby.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2olyirxbc.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qqohshgv.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xkgtgbwm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pcbvhzax.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rlfgpbjm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qmlgqqch.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2duisniay.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2kzkdnymr.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lpkayvwe.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cybjedkh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2togrmmpv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2lhwptfkz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2pwxbclxy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2uvhbqhuv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwxmbknb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2rojbufka.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2xonxtsgi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2emngmirv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrmizvek.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ofsvuqeg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2idfmcyzr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yivvacge.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2idguqmje.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2krfwzunm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pilkijhb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pfnzzgjc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kmfdhkdb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wcfjlswx.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2nucgrvfz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ubycxexz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2eubolppu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tnkwxhkq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fhniylsh.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2vvsboaab.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2lmfsgmyu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2bemtuotl.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2sslozfqj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2iqzavgow.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qddyerpw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2cxgaypxx.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ecgjlphz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2qvxmrfpu.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2kyokuxir.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pvzvuowi.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pxraddbj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2vizzpigl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2zmjpjkdm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2jroryppg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2wkchrbcd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2gbwtslkc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ngztqqhj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ekscefjo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2knloxqcj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2dpalqgho.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2jgdnndff.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2bwsxjpkb.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2besswdaa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ccpcefrs.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cbwmcxjy.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cremzudt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ojbyoyje.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2otcjmeuu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2avxuktiv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ahsnnpcp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rcnhovtq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2omcogapn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jhnakyri.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wmsdmysz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mtbcusgb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2siccqlon.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2yhxagywf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2cprowkjy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2lrivshnm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2macobife.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2biofqgtp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2uvdwgajw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qyynfbgi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2onugmwac.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ekxqddsh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2epqbxbev.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rlojinil.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2bqelbzum.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2uecmrldc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ejvhxnfw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hlwzcrsm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2irilftkx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2sztweicj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2qvyqzypc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2cjusdnzx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2bcsqmhtw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bmtbkuqj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fzkrusxw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2addpooxc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mupkdvzh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mnnnqukj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bynkrgbp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2cvxjlgud.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpsgbkpo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2hzaumnaz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2izxpkukn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2nybxsqkj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2hkypihma.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2jddonnia.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2cpuufipv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2fzxmmcto.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cawqgvin.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2vyuqshdo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2pjsfsykw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jmwgcxxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxirxxgm.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2uhaiaazu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oshibgur.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2rxoltvbr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2duaxnfnj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtxvxzok.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jsxcsliy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pomfseue.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rriaubpf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2vxrqsovq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ofwxaeix.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ghdmhxmg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2amwxrzde.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2gpzudtmc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2utysopok.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2numeucyi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nselsvfg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vunpubzq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2efpmrygj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nmhrwlrh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yqydoaxk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2vinyypkp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vegjhjiy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aqhbvpmv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ezpqzisi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2huoqpokj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kssnwggy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oyxyeoos.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2wtdoiucz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ilxfvukd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mahangsw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2eraftmqb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2dejwgzny.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cusgjckj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2drrudgtj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2gygmajag.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2qcvrmzso.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ktkwmslc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2olcpjkil.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qmjdfnku.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ptdruisp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhimkffi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wthcfwnn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmncyzzq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmwrtame.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dzbelhxp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2kmxxvovh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xvbdctie.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2adlofatr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jvixuoye.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ygsfbsyt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2prvjluid.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jaqcadmd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cphuvhxr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ptyxedyj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2duitqapz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2mtykzdcr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2jweaqmll.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2vncpmzqs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2nqsznypp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jnakiinp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2trrjstny.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oulbuwab.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hqiyoedg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2bflrrafz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyisohod.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2cdlmvgzc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2kdafdqoq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2imigvzgz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dvcysqay.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iiniekly.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lwcbuslf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cgrbndsv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ferjrosn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dpnwfmgm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2shqoidol.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2xfqgaoia.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xthklbpt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mzqjqloc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ucwwbdjw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzgteolt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tvwgbkch.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2lonmunqo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kqvsvhpp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2khgzjxcv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2zprivtru.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoidkcoa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zdvqdcog.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2eioollky.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2odehqraf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2unfrywgx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bjlnvmeh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwhtpvjz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2eepzswuy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zlyezbkr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tmgtpduo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ojsnbsnb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2emlaiwhp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2fgatcgun.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2oxlihube.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ssubsbpd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lgwesyuj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2euoftenu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2eajvlszc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2cfxihjop.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qsgaogyv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cwjqptdr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2blutwmec.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qicpjwhz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2uxqgitdj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mmzclmnl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2rnquznjt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2etmbfqig.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2iuzthpau.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fxmgtkhv.html


<!-- 参考信息 -->