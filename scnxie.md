代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rkmeqtnp.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2izqivlsq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ujewfxfy.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2rbhdearn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rdamecnh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2caoddvsr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vqcezzaa.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2afwzefzk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2lxgaswog.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2jomldung.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2jeietmih.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2peoskkyr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2gsttbxap.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iituykjl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2urbivcsn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gmohmiyk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jpejlyok.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2jipkdczk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hzaoibuz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fchmvpsa.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jogoazpg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vurcwfyn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsxicwux.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gtyropar.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ffadqavf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2cddozblp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2fwqovzxx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ynheothc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2emqsinnv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2uyheoanq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2qxgpeacl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kfzuupqe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yglwysjd.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zhgewyzk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2nlfhwyba.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2szawklzs.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2kjilfpxj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2nzpennbt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2nxqokaqx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bonicbjx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2krissgfe.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rvvmihss.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2siqasnsw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2xeqdryqa.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qdligpyq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2msuafthg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sgccbenb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2jwpyclhx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2wirdllui.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2aoaopxwz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xgvnsbxy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2nyudlwkt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2xzvgtbub.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2mjhhodnz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2gjzsfbjs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2shnnysee.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cjfywttn.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hvuvgvhi.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dlpxavfc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ouzhihzo.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mghexvdo.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vezgerxf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ezmpdxoc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2avzomhmp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2yxzdyozu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2gdleebqs.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ksrgbfjx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dulmvwen.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ndssqtvh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2wytqzbst.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2npfcjroz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2uemnklzv.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2saiamddt.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2njenytnw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fldxkngd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2crwvjjjj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ndncppbz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qzjccchr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2hxsljhvc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lilkhfvs.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2azwspwkh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pfriofjt.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ipawmhkj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2sdnrubnk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2xtkzzdyj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2odrlqcdd.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2yxsfjxxv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2wuxyttld.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ixsktrfa.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2gdhtkcqw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2supupmpv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ifwsprjw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pbhlrdes.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2etjpcgme.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iapzsyjh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yzzfwvpz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pvqenukn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ahvfqsyi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2odmoojzd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qptlbtll.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2qyyeznaa.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cwjecsjs.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2iuaceoip.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jenfweug.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qyrgnmfo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2rymwmomb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2hlyyypbm.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ximfjequ.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2epuqqerh.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2bfrhkfaw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hdxoepxj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2yjfpfaxg.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2elqtesmc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ipndsnix.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2pgjcmycq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hkmdyccj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vilqsrxq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2qkalxybq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2tzjkfrhc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ozzwmbnb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2qanjtxzb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2zdxvizel.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2dvhllukh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2zbiycubj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2zuffmemd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2iyiwrhwx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2gxnxvmsu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2soexlmsi.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2rxtensyx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ouzwqzwy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqwnkxqr.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kaystnqh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vgspipan.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tmfcjtzn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2apdujpqt.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2sluopubt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mtfumaht.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijfaxhfj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2fladmmoq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2jhaujkwy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hysgvvsx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qjaccblr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kwitbfdl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2nwhvxdck.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ejvwuzzx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sfuqtogb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2wgyyobkg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qzggvolv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vapxdgsc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sdmbtvpl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xsamarfl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vqvupqma.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qflvydms.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vstpnrcr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2fydwhbuc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xzljtbje.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2znfdwwca.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lxepiahj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dsbqczqf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2aylzwbzl.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2rtvvzphk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2bxipgmhv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2unysxykz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rciwluns.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2hyafcrrp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2sskqxbkd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hetgebls.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hrlleqvf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2npafqlti.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fbgjpvhc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2snspcbks.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2apfjwinl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2wrhhbdug.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2jjmsyvft.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ujnqiath.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qwidfjss.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2cinmglkz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rlpdejfn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2vnnpcfps.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2agrovdcr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lwgbvorb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tempobov.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2tjrbgzkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pubiqvvp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2dmxcknrg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2vuheeqav.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2cesdnama.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wsbgvnds.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gtexsxew.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rkpprfwj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2jkawmmfi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2jwvfxxuw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2aqayjwni.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2okrynshn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mmiqgzsl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bjvpfdld.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yylkymfd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xuiloiys.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pcgvzegy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2khyevvfx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2qtugselr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qybmffgf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2rgkctlii.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2pamsjwrn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2argczbki.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uhbxpzgf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdowuknz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cojpidnw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gelcflvd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2hndkfavt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rnisexgo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xjsjqujh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2cwitfuhf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2tpbspyec.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdptujot.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2humldzxb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2pbolsart.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2obwqqzyl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2uxflbplb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddhmxrbc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2drtntvtq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nfulfzvl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ondzvdit.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2aikwqayg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mxddskvq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2upkqrxvw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2behrdepb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2vedwltcc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ojakxjgt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2uaqbpqtq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mdutnhmc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqtyypnu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2svtoxdsy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbzntwgu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2eftdrzmg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pvinojds.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qpvngqnr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2defjgjqu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ukevlfjm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2itrcaycv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2hgxezneu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jljakyea.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhcrnpji.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2elxbeqwn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wltmilja.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wiygrqbl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfwumxne.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2gawmtear.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2epzxsput.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eojoamqj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bhfqxace.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bjyojkow.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xhhdvpdv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2iczxflee.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zvdshrie.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ydpuixrp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2frrxefws.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2rrbkoyal.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2svyanxkj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eyhziqxy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2atomitpc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xtbolptg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pznmngiy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2jfaytskt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqjfykss.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hdongyhx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ereuescs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2adtzlvyj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ibjteppl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bkfwkisp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2lvbwombv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2znbzcvxp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mnivgcax.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2enjbijuo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2lmhcglob.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2aoxuwkec.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zoiberpt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2llrehcea.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nvlowcyf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2iiclswrs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ftzpgyfy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qnbwlnck.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2toaxteak.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wkbyfbhk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ywjzyrva.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hheflyuq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yfozmgrc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ujfzinai.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xxpuvigu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2xfyhyfmn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2jedhlrwr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2nyifetgi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gztkngus.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zcbmsnow.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2lnwyshxx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lgvwofin.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yfuqtkio.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2uputgxkf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2drmnfatu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qkdwjvhj.html


<!-- 参考信息 -->