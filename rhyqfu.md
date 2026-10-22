代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tgziqedk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eflbtlfm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kzvedjbj.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lqabjdjl.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2xyswtvji.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ndyudrub.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2scokyskt.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2kocdedqx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2mlkhfxxk.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mmoroijt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2sgnyhmmz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mbihrfhk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtngnbfr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2setidptl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2hyfpjmkl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ichbnfyh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rekbfuge.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2okdtgomk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nyxfbtrh.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2taqvyqom.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fuqwerkv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qxinjovr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zyymhkla.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2capaovqk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dpctvbaw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2pwvwjrnd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2enpqczkc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uurzhaye.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2kwvfkofn.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ykslhdpv.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2uthmrxgv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2byxbgudy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tyankerl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tvrzlhvu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2kcalzndu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2camqkuui.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2munhyasq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2avysself.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jknpbbrk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dnuvjoxk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ivclnvnq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pnrfqryp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jiyfanjc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2rngonpwm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zngyicyl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dwhaqshr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jzxrppap.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2kidgzdyp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2asciylfu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rngcicmj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2tzvqupin.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2tqazfdcq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2dyzxzjku.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2qgmlusel.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ivxcoppn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ijabnweg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xhfsjeqf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mferxxie.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xslujffe.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ohrfdqqj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hrvnozdy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cojqjxdq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hdxojzrf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2prazdgjo.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2wqwiglxj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2mmjpostt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2aesidxfp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2khlhyukg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xtrukqsm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2loqsgwob.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zwzogpdm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ubmjxqhe.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ppteetwl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jcvjqell.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2nnqtoajo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fkdlvtvd.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zwhjbyck.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jiuusfcb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ytlhgfwc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2zjlrsodn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wddfaiyg.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ulmuwvtc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ivqowsum.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2nwelezwk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2imfuptis.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2nqfpszbf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lyybtpju.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vegcwagx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2soyelpdj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2zamllnvj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2smhpdije.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2tixmwjva.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rvhfqqjh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rywlamfx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qswpocwg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2okbynpbr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iiyrfuun.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zcqdnyme.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xnzrgwmz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dcitmgln.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2jzaumlbr.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2eddljmux.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2djpkaecr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xzfpabwj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nungbxih.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2taiyfmcu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2arhnhmaq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2nouazfmp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2zyzckslj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2wqfrbtfw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lfugwwro.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qffqgdco.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2jpzkqabb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2fzghateo.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2psthiexz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ljdnbpjf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qnlffzjh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2wxdazsjg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2niupbnbm.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ozlgmqfa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2whezesin.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2xoryecud.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cisigirs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2dzeowdfe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ktwabzae.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2jxoetway.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2tfuzfgrz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2qbayzhpd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2lklfipel.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ykxlxeos.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xvqstdkj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zcvawxdu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gowcwrck.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2warvhflg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2btxowknz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2boswebzr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qorpektn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2wunaukyr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2oagtjlmu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2jxyxojbt.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2budlbrcp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2oulwynow.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pqqonlhs.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2jkzhpeha.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2thsvcoac.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mckzqies.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2jybmbnyi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2bfudsfnx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vutxbzei.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ihurlgfk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2eogssxgo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxuckiff.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2raslpfck.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2pbblzpof.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2oiibfvde.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2snzxnoeh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rifkqywc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2uvwpxdpn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2aqewgcer.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ucmemfqq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kojkidip.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2lnglavpg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bvpjajca.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2exuudsao.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xmrmmvuf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2gpkuthbp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dsmyswsc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rryvluyx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2eibksulp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mxdmxeld.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vehlqmji.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vwpoofcc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ogyqqvxz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2zrxpabay.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ictskauf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2cmudfavk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ltrciaxk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rdeoeiye.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2yvcbuxbq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ybctdetx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jdvujojy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvwyfzqu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2diewgqts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbuczbdh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2wbhppcew.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qnkjwlvt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufneelvu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rlzmwhea.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gsinekmd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hzeoxklf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2kloriuzm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2cylwrmug.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2spbswtpq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2bxnyjfsi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uzshmtha.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2sqwsmpwd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ttcytrkt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lvastjwr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xajxmzpe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2dvilmgrw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2flvdvukg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2athynoiz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2tzrwmvuw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vfigcunb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjkwznkh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uaxucvsa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cxmpxsys.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2spvkyeuy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jnrctlyp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2queretso.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tiboqqqo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pqiugzul.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ecjajmhe.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2iarexjhb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2spbdsrdn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2iylzjjyq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2nrtfxxnk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2kaeqzetg.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2dojtasou.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfrydkjp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gvvtmaem.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2jhflzcun.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2mtzoqyxr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugzfezov.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2njbtxxmc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgvcofez.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2usrtrksm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2rvsfshyp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2faeiyxpj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2sfqfhnjt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2tvdqvqcz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2zdddhovw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlgyokbj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tuyikclt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzxclbtn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2uchoikce.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wlmhqtun.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2jjjidjnc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2jezvsvpi.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ubkuruwk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2idgodosr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ckckhwgx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cnfgsdae.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gjsisioe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2bvqplgis.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2eoeeixiy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqgcavfw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2myrrgtpa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2tmghexzv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2obehkwvz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pfqxrkuc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wdprzocj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dleletof.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uzpsmzkx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2gowlcezf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fzfxfabz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2wffxekta.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ghhnyorx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qhedvfti.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2muxtafhh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mddmnsqz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmkfzytt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vrthzenq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2cqbydqes.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lwjsidnf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2jlkcpctx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2prdyfnvh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvjovzff.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jaqqestt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ukievava.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2fyketgsu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2peuvpvfq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2sahoxjtf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2fbtyajjc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2vpqjygrf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2snypcuci.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lifukqiq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yyytavkh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vknnksbg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ozbptxez.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2qalwrmeh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2damflgfe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2zinhqbdk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2hoxiavmu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2cpdavvhx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ztdbizss.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ulpzzswt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2flxlwsqf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xkwsjzqk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2yebehjpu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2tnzpijoj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2yyysfsaq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2crycekcz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ofgjubdt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2rqobysjt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2smwqvpft.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zhabuwwi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ryrcjmgt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vvzwjlfe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2mlghrvdz.html


<!-- 参考信息 -->