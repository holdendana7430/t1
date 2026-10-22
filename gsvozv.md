代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2nitclmqx.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2pltkzewr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2wqdtgwwj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2wkpcwwkx.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2mxsvzltv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2lelfltsx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2fjvppfcu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2skpixgcd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2lhhlelre.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rflfhfim.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2soeydsbe.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2upapidnl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2alcbuejw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2mkztieop.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dlsubvgt.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zgzudysi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmucwxvz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjbsofur.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iiiwwace.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ccudqdpa.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sufommzc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2wsuddnnr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ihscuvka.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hqvffpve.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2fuyakrlq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2hsmmexjc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2rtzdktij.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vsmqgwtg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qibjzivq.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tvkmmxrr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2jnzyronr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2vpoapamj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qodljgfj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2svmpouqe.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gqbbxqqw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ndktpcph.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xcorohoi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iijxusmi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cfjefdby.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2uqqcrgpr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bopjvjxu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uyyvpoyf.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2mcgsoufj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2axbhkmuz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2oprdfdin.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rurwmhth.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2hqcrhsmg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mjycqran.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qhpcxevv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2estpeapl.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qwvyjlaf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ufwzgcuj.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pyadsacg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hoeyotaq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mvirenqj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uzpuutym.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mxgiqnax.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2empywmtt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dzrsgqdo.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2athargau.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2spaiwiay.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2xeueyjpo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2oeinozxj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uqoybdem.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kpilxtpl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ipfkjidg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oagohfrz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2uobtamqi.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jwgsvfuh.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ghxzapwp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2oakshklx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2psbnpnuz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ljqzzpye.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cffucadc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2lnyswdzt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lluqwnqq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2whfloxeo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xyfirhku.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ogfcyffs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qfimzzww.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2cdjiakxg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xxrperav.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2spnetdtj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcxalkmw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2vaifrsnz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2yvkrlcua.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfatysuk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2opgucrcr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2znbwlmzi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2moboxtvm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xnaeyugf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pxeimila.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jqkrpoaj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2btimlsij.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2urfesaiu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uticgxwv.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2vtpmbuwy.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wcndqxji.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2iznqfoyh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2cjypsjdg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2dsrtaqav.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2hjrocpvw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2thucbcbe.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2nazpdxlk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2hpsnjolx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2oestagbo.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gudbpkak.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ccrwrjdm.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kapfdjiw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2krxkuwac.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2epdkeouh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ldybtrgb.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vmecqaao.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2yygvdstk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2dmnnrzqp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2qgzdwgou.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2djgrixzs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qwffakkv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tohcwhcq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2cifsdhrh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2tbdlfmxe.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2vxrwqnhu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2yqhulomf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2vmffrcjp.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2hnktizvw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cnwifmwg.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vodxagaj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rquubkyc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ujemriop.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fcjtifnu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bbllcukj.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2mwzygpwq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2slzfbuyy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojccdcoa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ccbmbrsr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2yhzltawe.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2dklhizcc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2mdxdnhgs.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tgjvioih.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2onzjrgbj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2zshunvmi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ujuxncdk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2giagkqnb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2zuaidnud.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lqgkgqpl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2auxnfswm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kmbeloqk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xlhhibhj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rtcfygwf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2xvvratml.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2lenmycaz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2lwrsjtce.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ajvbxqmk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ugdefown.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xmefppfk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2eixqjotr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2iossrxhc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2xhghcwpg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rtijbgyv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wcuyeoai.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2bsndvwsx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jtzeysth.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2nkitaemi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2iymmvrsg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hulnjpbk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nprhduoq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2yhfsabxk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ikewjyrf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2wmrsazeb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2edfjepgi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2sysfwugf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2wnxtbbxl.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2lilxljcf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2alnngltk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2eduxqaov.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2guaiygqp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2kwkgycku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmxcyggw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2zvsawgfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wudrvvad.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2twxczcbi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ebgpumsr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2haieesxd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gdhurrjk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vqmfjpro.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ppoarmwy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2gvcnwcci.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2iidhjrmx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cmeckmar.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2fazglvih.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2oexumwlj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysquaupc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nfesdjas.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pylgoniv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gwjunbco.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2srqesnyw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ozylxqww.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ghgqkmdo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2varxsqlc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2yytkfjtf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jhdbafjc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ffhtzquu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wupjukkk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ysbjcsyq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bbbiqixr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2gqlsvbwp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nzdtjxyv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gnvrnalj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2omldkils.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2adspitdv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tqnsfjcg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozkpnwgm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2qyyhqzbd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2utonckru.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2pkjdndxq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvguvawh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2aaverzuu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2lfntjyts.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2cecifsad.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhhetbef.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqtbpdtc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2plrbgpko.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gjoesbhn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hshynwrv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmbljyfc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2pfzdttrk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2oxhyligp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpjrdxrq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmdkzkuj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbwcfnfj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbkodhjr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2osarxjyt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2uzdytptn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2gmjfzagd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dklxpgmo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hgelyrfq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxsqfovm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gkwfksov.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qewysysn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfzrmqni.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2uwqybzfa.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2gnewxrcn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ognjwqgo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2xqvjcper.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2hkeirfvo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2romnqayz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jysqwutt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zbffozhz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oqctiltg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jtawjicv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2eenwsqvy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uzvhbqsf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2famdfesj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2woxzfetz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kozkeoij.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfxzydbe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bdcewnou.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2phtbwaow.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2yktgfsra.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nhqhdrju.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryxllqyc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2mirlhoxh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vdukncvk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibbhrxcb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lftndomv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zatyzbgn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdftvilm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ollovduc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2stufoslq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsfqzbmj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2pperviup.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2pbzgcqde.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2fgxgrkpl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nafchlyi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ijqykhjc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zvhmqsfi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2scprbsln.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rbkjrmce.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2owosxidw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2odxepeuk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2sscqvgks.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2eypufhpl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yxysitbh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qjyuqkjr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lywjhxpd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2rjkglxus.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2hvrrdiyt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2oezfysjs.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ukxhudmw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ojejxkoj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2cwicjguh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kgafzeqz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sfkdkisg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2uuswdxcc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tgntvyxl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jlqpkkum.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ofdtngew.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2fevvuojo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2akhrqtih.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2jhvdbzee.html


<!-- 参考信息 -->