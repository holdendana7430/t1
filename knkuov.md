代发 wailian999

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2msrjkfwm.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ldvgrdci.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2zpwlnopw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2scofzijl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dlctmjbb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2psjlwugh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2rhkcwziu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2xzefsjyl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vllqgvij.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2teluisky.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pvnlavas.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2kheopcyz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2amicwiea.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ydmbnbeo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ledqbeqq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cnpraqsy.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2cgtpuudd.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2extiiupw.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ydojtkxe.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fpwhrluk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2qpiumxyj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jpsbdicj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2pyfkdrku.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2prelbhpp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2avrevigq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2rjxutreo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kzzshskx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dbpojdrl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fgocjcxa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hkrksejb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uinlhfjl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nhkexzrd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nwsaqbzi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ewlthhko.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2wizcejot.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dpgbmqtr.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ejitlhog.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2pfpqlbtu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2bkqzvxxw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gaevsart.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fkhucrwe.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lzpduhky.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2mnrajvdb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2xmzaocge.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2mswhohkb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2xlwuxdsd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2yfkqwumf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iezbxeqw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lxesdbhd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2igrcfgmt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gilbdtwt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2sxknhpab.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mhfrrlds.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vsuhvsxc.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lzdjelqw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2fngptcxy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2furlphad.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kzexesqo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2lhxpkzae.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2azrmoqnf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2xlnptwxg.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qttbeluj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2rumaisso.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2kijyjuxn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jszmfmie.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vhulxhki.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xlryrlzz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lwfstozq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bqybdvdc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fmecdlbl.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hjbahtho.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yenvdrtq.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2bdzxgtpm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2okbiszzk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2imtgofly.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fbmyjjcw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zjdeuikv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2vpqkkvio.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dluhpooc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2wbgrvycy.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hsmwzged.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2sjnxjsvi.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dwsnalim.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qvqavehe.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2awqmfmbt.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rycwbggn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2fbvjrrtp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2wbwihvbz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tnzlsybr.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2inwbcqqq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qjgyubwv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ykocwnol.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2racozmsl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ujippeol.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2maotqhzm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2eitojvao.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2rfwtuzpd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2fsltdkmv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2fenjhtzu.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2dukxgqng.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lxymuhzw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mnelvhcf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nnzogfnh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hxukgtfd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mgfrcfrn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xpseqgfw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tbaolbwa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rehvvzat.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2nbtdgyol.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pfzljkkb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2abwqcito.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2oiaxjwjd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wdbksixv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2psxhlvzn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2rquwaqil.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2vuxthmcd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2mbvqtniy.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2wtlbsjnc.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ecxmrngd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2xhbfaqto.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ixaoqmhl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2eajgxxcz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ekqgozaw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hmvlghsb.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zjpirsoa.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2iqhficqm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2abniiytl.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ehqxyvbi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2anytuogz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2xsioklnr.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xkrfzmzo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vrctpfvq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2adnrukot.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2lkcncnlv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ihgnquqe.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ybaulqaz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2jyhcmlej.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qxwncltx.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2szlokjvl.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rrdckixs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pbavpzem.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ppbnmhbm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nbickbko.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2dwalqmid.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ltqwspnq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ltdrxjtd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2hrsdulrt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2zjdkygew.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2lcttygux.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2mxzarxqm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2jjflmydm.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rdwqpyrv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rautsqzx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hsbszuhu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2rtffewuq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gteasszf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2adayrtjp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gcytxhun.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ygqlqokm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2pjetyirs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tfokkdrd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2alidasqu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2lzcupvaa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2jamrawsm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2uyfsufvb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cinpnayd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qgwlsqwt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2corhouka.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dkbyafvg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2konckfty.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2clpngehg.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ilazamrw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2tipgxtum.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ripvobpr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cdawbatw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tlotfhxt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2waqeneyv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcezmsyr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2bhmpeefo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zffrlooj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2gvaoalgi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2rblbprkq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ihzzkuni.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ymkvrkoe.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2baxjjdrl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ngciqfci.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ozkebvay.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mogsuecd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2bcsovqvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dopaoipu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2iwyructv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guehvnvy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2imhobylq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zkczanil.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2oagcwmza.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qiezxckm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2exfnkgzn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vpncinju.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2usxfmuxt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2txokwhem.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xpefbcvm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2jqrljqfq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2qostgmsf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2fepgiehx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pakwlorm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2iwpckukq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rbfnlwnd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ievbazpd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2unnqrsti.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qqemmysc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2xbpcqmbh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2rszhxztn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqvllmga.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pxbulhbn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwbzovvi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmuhldpe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2unqisvct.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2twuaikdk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2yyusutgr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2upxxmtnu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2btdujpde.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2kgbpmoxk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2obxkltrx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuanneko.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2muqyyxpw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ohkpyhxd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kkbkcmik.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fafkfqrl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jzghgzou.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2vjjhlvug.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzgxahxk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ekwgbdkj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tetvjfsr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kaazozsj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vdweddci.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ijkysraj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2bzjrcdjz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jtrxegwn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jbwnezla.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cidkpjqv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cevbrocd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zxnakloe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ndcwbuao.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2xdxklqkn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mmetdrtp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mosjmvvp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2wcuaocjn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ocqlcirf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2joezggss.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrybnstu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkjtefxb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdeyvldz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2buiberam.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2lxlmwuvd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iyveevfr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2qktjhfut.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qkzzlobc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mumvstpt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cpmaxzht.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cohgcqpp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nqchwkfu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ecvewtfl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2fczypjde.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2silkwuaq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2krtbqbxb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2grcuguvf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tucyctia.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgunzcrh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kganzdvr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaxnjveg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nzlosboe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wnhugqbm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hdbhazcf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2wyfzxkov.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wdgogqxj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zqagoxue.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jnhbacxs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xpmnoclq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ltdtdkry.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lrnbsbbh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2kjcylboh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2atuuepop.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lweudpga.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2qaktxioa.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2miomrvcc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hjxpfxhc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2piszyfui.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xwlzvtjw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2oaezutye.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2arpheetq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2rwxgujtr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2tyzpbvfi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ztskwsug.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ejsiftwo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2irwvjdpc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gvjusgiw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qipjoiqd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2uvytwzow.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ugidixuz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2eceomove.html


<!-- 参考信息 -->