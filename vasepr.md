代发 wailian999

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zacpxuig.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mhipjmpi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bkmyvlbo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jypfcaam.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2sbzzobsi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kjcpiwys.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2kilinzai.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2anweuemi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wulxbebs.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2zghlxbbo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wkiumfus.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fyfdohbb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mslqxsjw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pgqxzrtz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2prcvkhdz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2dentsmdo.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2botemxdo.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2gnfqyijw.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ovjkwrvj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uiwsaznk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2zfgigqhl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pwlttfwf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2vjtegnqm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vanzvent.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qxspyuov.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2mquanrui.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xuhavkwy.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pxnlvxvl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfeuviei.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2llqwvmxf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2feyshvbs.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ljlaulfg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jznvqxio.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2qkfernrt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2doblssvp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ifhyhgxe.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2okzgecec.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2jtraqval.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2eleefewe.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ugqquodj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2liyfuujq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2duyyptms.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2hklpngyl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2yvkhtvfp.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2nhgrihgp.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2yilnegcs.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2wnlocgdj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xvtvntbw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bpycpphz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2etbigfex.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mezzzhdu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2cqtfdkaw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vljiwubb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dtijqlaf.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wszfxucw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2romhdqkq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2kblnejqd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2cduycyfg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2gqnnexmu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2plzgprpf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kxghnkku.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2cwcnumnq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2zdycbbvb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2tswlbbsp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ssqqmaus.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vrbireuj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2irdbcgmg.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oniycomj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yjdddxhb.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iocpzfif.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uaylywvw.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nxbvvlpa.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ffefzgcs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2yospgrpm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fxbaafls.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xjvwakgw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tblvzkfw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2yelzsgww.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sencczgw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2gyfhzmzb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vdzkhowh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jfxzkano.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2rctydcrm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lotbsgsk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ivvxuxrq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hxlhpouw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2baivqkea.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lhmyleds.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2bqpugkpv.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2eezrgluc.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2nvtnmwaf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zcdvchxi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2btytaefq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2vnwkjvrm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2duobowzo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlyufwwb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2teucjlou.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2boinegmi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tixyndag.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2rbrzzmqq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ryudxhvb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2phvzlzer.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uhygwyup.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mcuzkaqk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hkzmoiqo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yjvdfhjw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zmnmtcas.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2msjunaxg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2hyebtisj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hwmknjsz.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2enpiunas.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xixsochp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2sxwtdvym.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2tuhurgxf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2tgsnhnwu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2smulsphm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2grfwcgxb.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2igqamffb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lyuukitm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2awtoaaiv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2eswudrpw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bbuwodwl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2lalszvht.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xqguptuj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hgjebtlk.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2vxpvprqx.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2gvffulak.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2beofxdle.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2zdmapoqe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2vtrxiidn.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2gzxphlon.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2sghgzush.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkelnnz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2hjwykyes.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2njkgfadz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2zidukokt.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2fspnrjek.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gyxyqgbn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ydzhanvc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mdkqoyai.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2timwlngy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fgvunwbn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wafhwgat.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2tjbvqemp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rdtyzqtz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2bmoydjkq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2mzkssopi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2fgdcoxaq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2swwjpdfy.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2kybptvwi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2krsgwpqe.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jkvmpyqs.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tlsvvpnb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mofysfhf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jqajolhm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jzkioogu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gztydbnt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hbcivmiz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2isjvfzsv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2szwfkqdu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wjuloerp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2dyddqkzu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2cdsxckzq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2whnmydhj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjhwveja.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ogshfnez.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hmaeoujc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ebplxibh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2riewiilo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2abioecny.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gkythfzu.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hezgaeqc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2jtzdxxzx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ifiewsla.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dswejyah.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xarbrrks.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wsxrdocr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rkfnisnu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2cnfalwlo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rtmejdov.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2yqlzglwq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2zbznunzq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2vdkolfvg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2pceqccpp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2uljvghsx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vnsijttr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qlfbpjbw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2btxmkbqa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2oooumotd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vguhkzyo.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2iumxrivc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrpvudnc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2abfnqrxb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pkkxpxlv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbrmueus.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xrmaxiuc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xgsmjghf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cofhrequ.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2tqofcgdq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zjfdxgiq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dnrupxqr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2krvwfyhb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2zuygbfgu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhzqnofg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hkwmnuma.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wlacxdus.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gnwlwqnz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2koiufuew.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2tekrslrj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bdblhntk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2wmgqclok.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2bzhsqnyi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ahhluuhg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ojnqjtye.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ywxyjkqx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rluddhex.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rktislow.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ucoxogmf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bspryqma.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hnumhcig.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bpiluanq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2wztwmbwj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkwoqhhv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhbwkhye.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwmrgqng.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2inqxzbxd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2tcizvumi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzsqqtfp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yqphdbrs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2khmikbgb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2iprlpygn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2typofmbf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwdwvwtg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2wfhcceeu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wtafpcbe.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mhzsunwn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2amwydvdg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2mwtxyjkl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ldkdepyf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfcuwabf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmkkibzi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bribqkzp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkizltya.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2bhamikvv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2llkhbwhq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyuizifz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hvcshmnp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ryngvbce.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzoprysh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsitufqy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qsixaojl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ioagqzhu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2qksyhshx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2brwkwbyr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rgdunzjq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2umyqqori.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wafdzoaq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wturnviu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2whujqiou.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qpyodqdq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tacdvppr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2eyvpavnv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ctvxdqxp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jvswgido.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2oqbvbdgg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jarlbtmd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aysbyvox.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hfzvtbiu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcxzwiyi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2evglyqdn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vwzpeixh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2yhwjrmin.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzrpejzq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cnwfkzub.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qfkfjwpb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ahlemsjx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2edxdlyhl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2adimsngj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnsawqcb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2hidzwcil.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2totnivcp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wbcjczox.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2asmeaspk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gcwooous.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rovcanvx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2soqgittg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vcoxfokm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2eraqnhsr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2njhaqrwa.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2dfviluzi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2svbhseub.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2urzomgio.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2vnqedorw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ihfyipaj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fxkpmccl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2akagnpyb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lceyrabx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2bvnhfdoz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2cdxmyhsg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2lzgezfey.html


<!-- 参考信息 -->