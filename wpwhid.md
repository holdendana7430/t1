代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3xgyoqesq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3kwldtjfw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qiosjprz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3iswzngws.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3bkscixdx.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fipmqalh.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3xtrtaqjk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vbkobpnr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhgahhmm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dqksgwdc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3zubzspbk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3osyogbam.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xzimzldt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ocvcasos.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jeepzjfw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cqyeqvov.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ntqpdkew.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dwlbngjn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ufgdkmre.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lxwzkomh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqcjiobc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3uxqbsuid.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3iqsoevul.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3talcscht.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3nwizlokt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqratzr.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3krmhbzfh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hebesfml.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dosgiiln.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pagwpvwn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3nzvcsday.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3azqgejaf.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3elvdvljh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3oxdadfqz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ysmlcafr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gajifdzd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ozhyxioh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kjcjnuzp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yugfedru.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3rbyujuqo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rncdcdmy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lookhxdt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3yneoblsl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3kbwbyfoa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3bxiphgpe.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rwrlxtbz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mpwzsvuq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3orifyqbi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3wgipbzxe.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zyuusqsi.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3mxthjmtq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3giymavtk.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ayhyfpri.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xeyyqrtq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ulgobggr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3psqbhzho.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ckcvnasj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eodzbzui.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lzxmezrv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yhjqofja.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3xgsunnlb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3myuabfif.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ydlmqlyx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lxzcldwn.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xussknbw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3oosyaeyb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hjqvwcrp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3jwjtdxsa.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ygpnrerj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qxbovgow.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3kjobtesf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dnpljanz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rcybtslc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ggxgjpgu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3hbnghrfm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3gpeoysog.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3fbjqeucq.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3alarazhu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3fnlskoop.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3corftaon.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3mprwkddc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3obzqiyfk.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxvxafad.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwbbtjcb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3jxfxtvub.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3zqpzgtch.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xbzamcsj.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3jityvgyg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3manqekry.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eayztnml.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uyghfmpu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnwnaorj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ducdsmbn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xszeeyav.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wzeasoal.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gkxkcbne.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3cglfpuyj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vkquvuzg.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3huqlvdzu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sdmwbely.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3amulhhng.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3xzxquwxm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ozafmvmy.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3pzkomfgz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ojoycoqm.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3eaxgqsxd.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hlghvxbq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3akqqkybt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3uvmmtoxa.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rrzybrci.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3weyqugjg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ksatoabz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3izxcciax.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3zkumlkbi.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3vfnlvyno.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3cnsonsjr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3fdzfqtae.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3aeccsmsj.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3unsejnrn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3dndfsibu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3bqwygsdv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tlnzkmfy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3gizhyhic.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3aayhdkhd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ljirnqah.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zkkjlpjt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ggizrqxn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wonqtvdz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xrcivuap.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jbcmkezt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gljirtek.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ilbofjjy.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jjvdncts.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dwjsogyj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3wmfupfyd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3psljcpow.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qnoxojvr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3rbypkzpl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3pbpfmrkb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hfitiwku.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3plbunoxb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ddrpmxze.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wpraizqs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3tjklynyu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ntqukced.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3svtuflab.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ntxddycb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ayclndkn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zezivdwf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3xedusbej.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3vrmnkaib.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3wwjbuypn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jxgkkfop.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uieikmdh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hietwdyb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3gukmnhny.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3cfoyjsbn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3vpdivder.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3monzwbvi.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cfbjuwxe.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jfdlxrnf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3okbzhasc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fdfvqdba.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3txyhuqwa.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wakeadyx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yamkggbp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3epewgzka.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pfnleqlo.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3blturkln.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3eiqhsvwm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3kedprbwv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3nkegyvmc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3kqhvbsut.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3uqpnxybo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3qjvagwxa.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3iqxyvpzb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gpakezkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upwyxlad.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3efcgajpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvqgtlhj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3qpidkhgj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wpbsgced.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3pqpwphhm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qxyxndht.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bvrtpqgj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dbsmafgw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3fhxsjwfc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ymwcqcwr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jtyjafvm.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3yxkegvxj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3vbmaftql.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrxyndgz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yynmimon.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xylifxpm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3eoiritqd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ullvaoyh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3udqmuivp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3isfjwwmb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vjyzvtwc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3rjwlsgvp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qatqbqiu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ecqvbxem.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zdngrdyo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwnrvxsn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hivaultq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3swjuqzuq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3iucwdbmb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ofoeyyrt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rvfxxanw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jraiivvi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eforjylj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jpdfedqv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ewruckls.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3lbarhnrt.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xqogsswh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qaawnlup.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3valxsxhh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3flruybxe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3roatopnj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lmpmmaga.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3uhynjmkz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbkoixlj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3dhovsoro.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xseokbnj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pynldpjd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xoezpnfz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3nkyywocf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rshtphsh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lcblsdon.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqphvirv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jyqijwuf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rxfruumd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3iurhvkyo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3fnsxakjg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3mzpgavyi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kkmwosbh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3gqqswtza.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gexmdnst.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3oeyoukyz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wesxawff.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3wnbibeos.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xlfhppue.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fxdpmriw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3xjwgffhv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3cewbaozy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3isiaaajv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yzsszxay.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cjhukfkf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oasigkdh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3olztwkya.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3xzsxbqxc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ztrwiqfj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jhbxbrqo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3oyhycegx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3phvbxvyv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmvjyury.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qudvcjqd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cnzqglkn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cqlzhfdb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3mrepmktf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pipuaadz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3rnvcvkar.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3wpvsvwsv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3oyozsigz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3twnjsdda.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vgowrjea.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3hzxwllbf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xltujfps.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wzxqnvzv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3fbllrsgx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mfpwqllj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3wfvgwrzu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tfhqcptd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3cisvnhtf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aauhcbpx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vswgsdff.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vzjnubuu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3augsapja.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3zjdyikkn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3xagifstq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3gtkovvyk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ppnjhiap.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mwbnfxmd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lbpciqsm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wsdegsye.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3xjeoiahn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3aqiqjwlx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3kbviuzej.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ybjtdheo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ddgncsus.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3gknvsptu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bripojtn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mcbrbbzs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3srcbrrpj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3pnhwhkmq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3fcijeckq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3pjoenodx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3uikzaxil.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3yhhbhllg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3gqsrkkbs.html


<!-- 参考信息 -->