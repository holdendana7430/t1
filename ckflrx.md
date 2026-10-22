代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cwsbvjel.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2nvtxncah.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ircgvbua.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iefxikhs.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfjvlsmz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ksfitnqv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2orfxjyej.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ukmugbjj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2syuwhcro.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2zzodrkoh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2dyuudzkx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2unonfezf.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2spyobcvh.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2wfawmicv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2dqvwhmmf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wxfmkrnt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tjlselox.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2atsrkqfb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2feuyujux.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2aqewnsye.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2givsqydh.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2dyykcagb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ncmdpwtg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2upsfkxiq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xmyiopnq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rykibxcw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qeeldmaf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2aatitwfj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ijqwzscs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ynfsaykd.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jmtipiet.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2nkcrofes.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2orrnemqp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2jbdkthtl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mrfvyoht.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2jyblvqvw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qfimacbc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2btwafmnk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2poogizzx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fdpsmcfs.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sosqmsgv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2urycnbtw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2romcplsu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wyvplour.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bclzxlny.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jxyprhjo.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gqjrajuz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cpmolzyw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2yxvmejtc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2xowlrhtu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2osxbqwvi.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pbqnxysd.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2csklibhc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2wfcvzliq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2prqrzbns.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2bosrlsel.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sjvroqzb.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2fvcetzjp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qgjbihqu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cfnmnihb.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xdterudf.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lhrbtspn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2mlzlwlqt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2almotkkr.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jirwdtze.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2trksxvto.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qebpyryq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2tcyeahnz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2rbwisdtq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2bjvdljdr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2mrsrxkgh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykykxhkr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2xlyojhsi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2camuheil.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrjbpoeq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2bzesfyti.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iziukhce.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cqpcmmcx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yajvetkn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cqbhmrfh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wrdiufsi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eaanfcho.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2izthzrjn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oyioiwlx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2iiegpzlb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2msqconkt.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2mmgaeshl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gbcogajf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nyyypuhb.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ffwqgygq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2advnbjkl.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2dihybjjq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2weztijaj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2dkhhagdp.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2oodypbdq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2kbeyfvsq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ythufaqi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2vbyaiaqk.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2sxwkmtpa.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gcgbphir.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2iwjmdkdm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2hyrpqilx.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2hdqccuyr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2cupafxqe.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2rzreyohe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2vthfolpx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2vayownbq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2kvzcvzuz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xuyfujsd.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2wtnzbwyw.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ccydwuya.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2hhmqgkpr.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zfozddtm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tvyofkll.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ollicddq.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dwbmwhan.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2plpvseyn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zpsbppmk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2foyecgav.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ontvltnn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bkvohrcw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ljkntbpk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2tusjaxkq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2vdtodiht.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qzftguza.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rmxhiebj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2vtcktfwq.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2arfnolxg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2qebgmfvc.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lilitsna.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2luuynwuj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2orkcwsyu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2afgsqlsu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uonuqjfn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2obplcmkj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eydrmyfb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hebvpsyy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2trcxmmlv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2axmxanaw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2wquxecdi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lewissha.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2sicvkgiv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bmhpprqt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2wsgdroem.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fdqsbewv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2dxrixmue.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2imhsslxc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jseucbuh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2jnoiqpga.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ogwntkfm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aojrnaqv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2casupjvp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2adicyrrx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vblcvqfw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2cvpsjxbk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bydttrui.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2jiurizwx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2wpgnbukd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2subsqllo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jiypfsds.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2lzrpzkqw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kwemxbqi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ylgrhcec.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lpcseche.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2lmbtvbvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dghsdvfh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2mtluxqxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzflszgr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2caqxqcbs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2idhngnxs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2pngattaw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rbypmpup.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bcwvlijv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2egqwlptq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2bscjgeld.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2jgtgtfri.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2stafkkbp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2pdkdyqwq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2zlmhwnqd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szredcbh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mglaxuqp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pixkkekw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2djzkrjdg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ekgknimj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2axbdnmzc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ojdgnpfy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2mfqfupiy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xjyjmian.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlruurkl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2awdjjnbh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2injtwvub.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evfrqxfd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2keghbqhe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2miopyjpj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2sxknsfiy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zqwezjya.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tsoxviik.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrfarbtj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmichkyl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysucaokc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvhqiuuz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2pviyowzs.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ticxbyzq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2gjylnvpn.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ixyyrkry.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hhmnucjg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2darubghp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2samdefcf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2aizdxlih.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvahjigk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bgdsapnw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2vqnwselu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mecarhnv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jlbmzzmp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2cvoxntix.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uckjrhwy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2orvpzyow.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bexlxoxp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2eepexzkt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2fzkfwrsc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2irwqoomd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kbjvnmvi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vuviptku.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ahmkjqtp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2msdeaqhu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2oyqrpkqg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fipywmpr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2chiylasl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2tsrcjvdk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2gghntdvn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdmjnxyc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2gjujutco.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wxqgxrrr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iyaqldyd.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lxqtgjzw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iqrwawgb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sberxwxo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2myypxedb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jctrmsev.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gvfywtjm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2znfwsnyz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qyheiwtc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gemiwgla.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjzsgjhb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2slhxuwvb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrifolup.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lwapsqkb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pugnhwxy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uraarabc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2frbqvhns.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2snjweyrv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2urqgxokz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ecknenoi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2klclsnue.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ryswuwmf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bsprlmzl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2jdyaglnd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zeiottyl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2dwppdisk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2yxpjduzh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2kadxcrqo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cjrkxadi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2petcwplb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ejuxtdgq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2lmqtfwfs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pelpfkre.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2blilzitk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hhxevxzk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2rrrveuva.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2jpmicnpe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2acuoriwc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xgppjpmn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2junixnwa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hziqfykp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2xarptqxl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2jnmvdnxz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2pwntvnkg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qtkfuvvx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2emzvcceu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qrryzrgy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hilpjbfw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2kedamdnq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2uwhclemx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ymcmtttz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2tzyrmmgn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ioivspbl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2bpngonyo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2plpdyxrd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymrxkunj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ucekuzbi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zqdjtvgx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdogbqcn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cmabxngw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xctorztc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vpwxudcw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2fudqbumm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vthgpeka.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vduwqwik.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cdlgpbwb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fqhmszmb.html


<!-- 参考信息 -->