代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qcrhyikb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3feahwdsv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3cnqtdjdq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3jxzhsikr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ztejosby.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dfygvuzn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3evclonfe.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rbrvdhlt.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3trjlbwaw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tnyriehs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xzpykjld.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3apvvczpu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3qsngaxhk.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ewgomapb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3wnefojax.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ghmrupte.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3lklekxhf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gstbgcnd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3zobpdlsl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yszllabv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fnijsmfm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3towvsuye.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vgnecalo.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uzqxhpzq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwazrhjo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvaemlhe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mcdwjuik.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ockgqvuy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wyednjke.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3szdgdpml.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3arbrgbsm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lxutafae.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3sqbgmqvh.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3qhwsitdu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qdnhbrfx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tepnvcvf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xbbhyfro.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3osvwssof.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3rvyhwbzo.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3cvoxhypw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3pxckoavh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3eebrwfjh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3auvqxwho.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ekavsupb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3svzyyiro.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qbrfrzqt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uiiuuxem.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3besgztwz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zxywjaro.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3omlayizh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3xokntjhv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ffqsxpxe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3xwyhpzae.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lohgktxm.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3wsuorxjv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jfsxexjr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3grpwphrm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3aoleljdf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3jyabbmbt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3alxoocnx.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kkmmniyl.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3scwisuky.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uugkyvvy.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3avnajlho.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oemditqh.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rtonszox.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3axiryvht.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iyjpvixm.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3gpttwosh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3iqhgrfbq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3leddcwdw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pehdulmc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3sptzvjdb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3qxiyyybr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hnnekbbt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3thjcmxuw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nztyrjlr.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3wtxkelbs.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pzgajpeg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3spzlaccz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jjrgkkht.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hgrvbtsg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3lodsihjc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jrlexbsr.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3htygobji.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pairzojs.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3sddlzcnd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3trxiebdp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rydwwpgj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3cfuifxho.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3nqlosyrb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3omhjffzs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3dgjcurox.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3yirxdisc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysqjtrxa.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ddgwebmz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kzhfswfh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nnlwrcgp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hearliwj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hngesyjc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iabrxehz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yiggydhp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3frfrzdyl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ytthhqmp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3uowwruqk.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jyvamypi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3sfguhsmh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pzzebziu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mlvoekfp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3mxpivvyz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3cboiicnf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3sfsrbycl.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ffnlebsc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3lcinfdfo.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3aqnckdjc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3nprmkuuf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3dpisheew.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3nfqnvvje.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3zxbgyqqq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ztcuczvq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vhfekxfr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3hstueyfk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3pdmkarog.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ztxbthtx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3yakvynom.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3zmdkdbmc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3obfwunir.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3gdbwgoxc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3vmzqiyrr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3nohiadtb.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3tfihrcks.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3qxhllcrg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3mcigfxbs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hfwxksyk.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jkdwdpbi.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fxzvqrcu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ytaazxrq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uafgnfdz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cbsxehzr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3hvrgrhsp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hfoprsjf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3voynfzyw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ylwncgpg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3akyfzubs.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fhglamwu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bemfyoss.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3tzxdnpgw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jytfzmtq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3strmombk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pethbavg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3fjxxutpp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3babgceot.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hifydlqd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fmakaxgf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3msintdvr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gduerzjk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wzzunpyn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3nmkjhgha.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3efdiscze.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3aipjzrxc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3juqvkzff.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3sychupat.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hzfqkeho.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3dgaixutp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3wgjssnhi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3fezsqdvv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ahndresn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3neyqfuqf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ythrghhg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zeqoziez.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vknvnbmo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ewpmipau.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3tyjqkkfo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3pckzslfj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3eyiwhzuk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvvjkwml.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3fbvhltuc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3idkiltxt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3xvasefxf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3pxlovvcb.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3sapzmfek.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ztrrxjhs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3mfzyxnbt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3djlxslkb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mbukclzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdddbdcc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ogpedmhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3govevrnn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3pkwnynfd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3flskqmak.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkwvcqqz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bsrkamxa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qnijiord.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pqzewgxc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3vnywajye.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xktyhmcd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pwbfpewr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ybscwugo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3kxilszvo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvwiacsv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mcakmrvl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zekpgqjk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uiasuwva.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3pkblwpli.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3hehqydvs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hbgveckj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ojfiudhd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3qcypbmnp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3egujjhsd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eddglbka.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hfhldzqp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytykbqqd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lbglzdgg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3kmoopgjf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xucbeurq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dpodzjlx.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ycthvirp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3lofxhqvq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ibfovbaq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcvefunm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbzfcrpr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3dtzmvrla.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ibasancq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3qeqjhxib.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zblpzscm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3gnmqtwvl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xthsfjzv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3meaidyny.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rrtomkgx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3kwhbtppb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3oppeztdz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wznckprx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3odkshilz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3pohjkrnw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3brbssyec.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ggejjvqp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bgrulsku.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iocumhcv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ijphlqjg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3yvyrxbyz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bgfxgemb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hceijzby.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3bhkwcden.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qhyimdoq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cahidzag.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyavzjgp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ezaequym.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3werhljir.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3wngxbkax.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3zjussyhs.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtrrzxzr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3yszhtdnb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zatmzoaf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vvjxugmd.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mroogoru.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zxbtmihv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3alvtrduh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ckiexubh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3nldbvibz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qmavzvis.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3bocqqyuz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3tgkuzpmq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3orfsygko.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkzmmuta.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xbaezvhp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xohjxsog.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jrtdxojx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3gfhqasib.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hirybtup.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3rtwpidyh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3okoubiks.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzikcffu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hnihgdqs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qwtleflv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3bttnwywn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qxwdesvr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xpjmywuk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zcycdrsd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3gxmiesdl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zftkwycd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3mdbbfaav.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qzpnvnht.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hihhbrda.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ruxnpykz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3lxydigiz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3lfcmdlrn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3yszheghf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3bargfbdh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3dfsmbnqb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3yqqtjzhz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gosktszl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cqvuopkx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fibzjuze.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hsogkwts.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rpgokzyu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ofjtbhia.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3vgehdpbh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3nvwxyyqg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tmeqnjek.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zxqpjmsx.html


<!-- 参考信息 -->