代发 wailian999

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hywrysqq.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bbrvqfjl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2lrshmgkr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dlwinvyy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qhtwyqto.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2crgjevgh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2iyqywhuz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2nnvgmmkz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2sjmohroh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2apikyfpb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xmaabpam.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hzilkvwu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2tkctvkjp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lqxmibul.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2qnmkxjuc.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zbxldqle.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2vizdfkbx.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2livuclpb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2mztgibcc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vigvvsij.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2cqotkrex.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2llreonet.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2spckesth.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qxbmjpyo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tznertod.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2sfsbcffc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vhefrxwb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ezmpjxgh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pzpjkife.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ipmwsedo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2njvmsaqq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2chawcfui.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jxvoswif.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2sggupzfr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2oautihdw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ikfpihre.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vecetvkw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2lxjnbnwc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2vnhxogno.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lbmbthuj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vpvfgbod.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fkhrylry.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ifogrykj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2niejamqq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2tybcllsz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2hqrxasdh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2btsggmld.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qmocnisj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uspazjbx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ibwyxrlg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iwwazhsl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2qvdepliq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iitihkqr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fhafdpbw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fxvmemgi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2byyhoxdf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2vzbrvkva.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rljxntxb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2kdjhmean.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jlxvfpmb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2kohhidpu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2phcfyywr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2xwztgqfb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2enpreosp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hncfrdes.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iwwolxzy.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uztnedlw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gyqzxlbj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vuetpgkk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pduclqtl.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pffgfyuv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2snjrpnfr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2meuvcsql.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2fvpndcvx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ynpoffez.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dmghmozc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gcaotzuv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2fyckvrss.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yacguybb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2rwjcfehc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2oqapwuri.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2frxrxdao.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2odqnaptm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2alxzwjiy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2oauplscp.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ngzwdmiu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2slujatvc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2rggydfwe.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2irrhljzt.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wtnbvtda.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2jgwmwoym.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2eofjlrvb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2hgxjwptr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2igyjkdyi.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2lrrvfohu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2qoqcjcep.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2bhqaisnn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2werjwkmt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2xbimwfcz.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2nsjorlbl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ngbljrvu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2atkhtzfj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gyxuvcll.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mvqxvpfw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bkxcsvsd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bpymizag.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aiwmyhdd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ugrcmxnp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ehidzpah.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2yyrcsdae.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dhqvkbjo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wrcsehqr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ypjbdgsl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2giwebpgk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2sdusrqsq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2peumnzgq.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2osuhdgiv.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2qhupsons.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ktqkaons.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2yrnpflas.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2szxmuilb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2tggqthgd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2zzzwyjqa.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qlnnvgur.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rfzhyhtn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2mhokyzun.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2uxxfrpxy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ojxvdkco.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ulbxxekl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2tzgeoukh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2kvxheczj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2afpawbyh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2tyrryltg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2wbiopmwm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ddasiyvv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2oitjnhas.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2aaypafbq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2iyocccag.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yszjgpps.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wbkxmngq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xdehrnst.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2figgazqi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xcnxtxwf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2lobkcovc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2acjgsieh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sdgfzeau.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2tlsacxan.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wpgtdump.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vqiuhofs.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ysralbuh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijjseyrp.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kebswtgh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dituljfv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zeikrwjm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2cxsqkanq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2enwqftgz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jywjfqgt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mvjmkkjg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2punrhqoc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2auildjnx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2blashypa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2lncjfbls.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2xapejovb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2drjujdyh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmjcncds.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lkiyqxii.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hmkkyute.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2eoctcxot.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2sparkmsh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2igebzrxq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mmadsjug.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2olejvgwa.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dhnxogms.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2psewvzyf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fafcufgc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tjtjshhi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzpmekik.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lossyeli.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2jqnqdxle.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsqrysxf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2bhvcnkkz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2whxxsrub.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2drphatfi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2tlpopbdi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2aajnctlh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2eswvkyay.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hjglmlaa.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xhbzbsce.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dahdrnqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drxtzodm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xxpgbwvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjxpwpre.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2kbcgflqt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2aigzvnap.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2huphxtid.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zaqxkwza.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ibygydfx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2udjjerdk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2fnddbnia.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hmumagec.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uyismgrl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2qomwgluc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2tbzfbdjq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhvytypk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nkwkfsce.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ojjkpvkx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ybmqgvtb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2lcgvfxzd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2iblfczar.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wjjrnclq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2njqgxonq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ywuurwps.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vxuqbnyi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eejinfpn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uplhvzcv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2grljkbkq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dnizivgf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zvqepsxs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sptfislx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lgsrxfqa.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2besibsju.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2kwbsalzd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rkviwsej.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yitjufuu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2htsyxxgg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2jhctzgsh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gntnzzre.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhljssaj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kdxoltwa.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ncfqhrqu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2sbxmtabz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ngbzpmak.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2llqfzszt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2fkzdeqpp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2oslacawb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2izshudsd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zmajdilk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2bzxdejdg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dzfqpikg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtokbpkm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mnaixhkm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2sazugkri.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2llqfqsln.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gliaadle.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wtaoobey.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2svyprwrq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ygyydxgi.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2kjhydjds.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dizwhmxz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ziivfcvo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnjjtefj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrhgjdgv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2hwgdcfqg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fwibpcfm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fliyowsk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2erbgrneq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zniqewhl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pixyzvau.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2geukrwzl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tzzqtfkq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bxorzjzq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xhnlikqh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dbtodmqz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ufvbpbpd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2wqjxbgzf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2msydapsy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2njindzbf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jaeqhlay.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qjoehkuy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ghbimext.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ayiqfoaw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2npyluoze.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2boxcddtg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cgiozdzu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wfixtxea.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuhfthoj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ygjzkovn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ptaauysm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2fatznowx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kdiqaotb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2lxblbefs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2uzwkvown.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ifeckruj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2svozmjug.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bhjikifa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nbibchcc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2trgrzxln.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ooblysqx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tjnioief.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pgdbjqnh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cmlbqkwg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lijdaihv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2irtzarzw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ajdnrwpr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rvvhaxbr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ddzqzvga.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2joebxkej.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2teetvotj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2etzwdeot.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2orjrhgmb.html


<!-- 参考信息 -->