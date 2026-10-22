代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fslgkemf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ypmufcxa.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2lnzawsxw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2lzxosoxy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gzyvhzss.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qdfsdxqq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ltcxdrkt.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2aqxtxski.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gjsnvoks.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fcybaryp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2uhiclyhw.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xrzshypt.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2jpsxpkaa.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2imnkeirx.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2omxxnkto.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qbifmhzb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2inkwaqoi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2outdeikw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2fdkguhgw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ckaiqgqj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wyfkixni.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2mrvqqsbh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wmyqrkga.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lcrmjmsj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hqxvuitv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jvnfhjcq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmpypppe.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gfpvcito.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpqxihmy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2qrdrnbar.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2qahybnlt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ieupmprz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vrmjqdhm.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2mpmjxini.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2pdvcpltq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nlnpbjvu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jmurzrfl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rznuacsr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2wjuikanu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2oesdxkqu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2bsxjslwd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2pclcfqwj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2emcrybnh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jrzpwobb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rpmlkblj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wavzkuxq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jzanwcnh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2xxcrmlhd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pqtcacqj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lmxkcsqk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2vgwldisk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2tmlouzvp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2xhwxvrll.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rzgrmyui.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2flientac.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2kbayqppr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wvndpeuz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2vwgbdqog.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2npwivxdv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ukoesutu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ksxdgbks.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qwrivtpn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uqbrmpcw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2soyampmx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yhsufcty.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ezrmscdi.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pecipnhy.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pbitrwru.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2fareflfk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2zmrvwcdx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nodfhdlk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ngsoskif.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2umewuaed.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2rrqrbopw.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ohgicsty.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ggxqyjrm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eboljhed.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2bghmsogh.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2bnjhsuqo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tiigqmpx.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qtgbnyhz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cehajlko.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2bbxdrhjm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2hmzykrlw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2heykjrdg.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ouwzrcyy.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ctppjhji.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mnzlsvmh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2whwqdlxr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2qbwzxtjc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzqxsjuh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucaybbso.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2cvearizs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2cgnaegew.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzqsquhl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2yqfaqhoz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ojgxzwpx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lxhlhtdx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mptnzqbt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kaiduejj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yucarmmx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vmethhvz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zjfpwbqs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jxlkogoc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2jsxklbyw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zbmxgbyy.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wsqwokys.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rhoiaqje.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ljgmjwwj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2bntnctas.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2xlgnewwb.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2onrawaml.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2hzhkursj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2mujkcrqn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ftgtptam.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2jiruitsd.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qwjcbevv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2airomwdc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2pmrhprjv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2altnxxpu.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jwdgozxy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2yjlnawvi.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2eyqwqkup.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2xsjbsuiq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ppudotxl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2wrdgfibl.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jvqqaook.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2roktbqjq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2cynjbzhl.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2msashado.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2dyzjhque.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2dpkplfro.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2mxyeambn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bidlixti.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wybryjam.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xerjubnn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mkllefsy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bfimlbkr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2aofsosaa.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2gzhzosup.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ptqakogd.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2mztfctbl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2sgedtvak.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2bfjislge.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2eklyzfap.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rrjezxjg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2rxosxvhr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2wjbwhlxp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2zzqzxjge.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2flmqwfnv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2gmubrlyx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ozjgloaq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fjpgxigw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yhtrbvpj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jszwcrvp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2amowbtvg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rcjasqvd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2cwyhgmip.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2wghecjfn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2hzdwdihl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahuogonq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2avqnzkmo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hrnkktya.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2uqvygsqi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2atedipwz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2nmahcrdm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nslowkox.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lvionjlf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ijyoljkf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2psusbhoa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pzasbepv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2debtiryu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rxqunxjs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyzzlhyz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ptivuplm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vbjqbaap.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2tqmdogky.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ywzcktsw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2kfhyuoec.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2bskqadqy.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2lzqorlkb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2crqkgxgw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ksjemhjw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2fhcjtxsf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wvlwonyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eojnruqs.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2dfxkckyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtshbqmo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ieiqpjzr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2rvbyvzaw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2odyyserj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xhvlhbsf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lhogxxmt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2utbyxajc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2fokxxfhs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kmdmqbne.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zxijxcwg.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2tdejiggj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xepmdqrj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mofjddkf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2igqsbizx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kuupvxzr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xxmxunwk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2drmtsute.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2etwfmnzz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fxnascgx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2jmphwsoz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2dozjnzqx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ruwktqgb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymhopsfj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uzmpidus.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsammhpk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wfmrwcqr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2jxcqlffa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ynqecqma.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2aoxynxoa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2opwqlyib.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhrrzxei.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2evaeaiyn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nhfelkqq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysicebme.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xhpijemv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2zmgxkgmq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2njckthoy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2obtfvepp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nvfngrtc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2sfuxomqj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmzndoyh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mnqhfrcx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zeympfgx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pjpnayqm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2hksgxxsl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhdrluff.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2hsbmnasf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2alqbykry.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkdatooz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhtluvfe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2iwkhyard.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2dwaoycgj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jijnsbwd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dcnkwzjv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkkzqliy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2fjvxsstv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2thhjnqwa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ooffsdrb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgoghevb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dgzvkent.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2igyfeyym.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ytadlrml.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2rlppdsbj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufmuarcm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2tfczncqi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dxlmastd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ljexxjyw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uqomphjz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2slmsjlpg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xbzknahy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kfkyrutb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2krenuyoy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bjwgcrab.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2kqdkljir.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hjzujrlg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sjmszjly.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gmaxsvnu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kycklryg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfctkenq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2oddsvgvc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dmwbnpqc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajoisfpt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2pzeidepc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2lbchjpgf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrckgviw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ftkxijde.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nwcceifa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsgisfsh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bahsxaci.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ivqpprdo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qrojulor.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2gjuhcfwb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2iywoujud.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2brmvasmg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mkqocbrn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2uoqvujpk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2icutdrfx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dzazubld.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dqpakqur.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2pdhnuzzo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ehkkywhn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2yxsxdyxp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rpzrlqkn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fiqolyeq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wnbrpuep.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2anngdigs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ycneovpc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2embtmfeb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2iglttubf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2eirnqlhh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xmjsirrw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ccdlkpzu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tururvlc.html


<!-- 参考信息 -->