代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zyhxlzxv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xbxuntig.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2nbmgszne.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2shfzliwe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2snduvmbv.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2smyywfiz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2nyitoalj.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2kpbasghb.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2hcnpnjjr.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2nlfcrnmc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hejxvxjo.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nrdagxeg.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2pjtdqhaa.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dycowdsi.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ftlyzmos.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2knfmynai.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2xrukbcpw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zxfbcrwt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ivuiumhc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vvaqsokw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2eilzfptm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2uftgeauh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qmgodcxn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hfqrpoeh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dwbrlxob.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uirtncbr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xjmyqwid.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vgpeorio.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vovrwgfl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2jgtyiyfo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2mvkjzzeh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxclshhv.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xxkdvnpl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2hbirnfcp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2olfqhrxu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xalioszc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ywlmtznu.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pxkvqsfj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2mstdomsv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2uzjfzdba.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2mbfbxhzp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2cmdeukwh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fvauhumd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gogwdpui.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tnqanfwj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eiforycd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2khxwbmpt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2jpcqhjar.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uhvzrsdw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2disliqre.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2voslsixb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2pmcsutzs.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2lxyacrey.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2nqztsjwb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2irnbnmlh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jemydtct.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ohiycnhn.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2yiezjktk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2fyverblo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2mypalwzc.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oeratvgv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ufikblkc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fpbxjflb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lpssnxte.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2imewgqgo.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dpvabjoo.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fwfzwdpp.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rwfxgaqh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2gqifszkk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2mwapitsa.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ombvvpyf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2awcfvnwc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2obklluhw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2vqayeccv.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ysokyzyy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2bmbqketm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cuvugkgz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xuafyigu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zgxszxjl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2msioctnv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2weshkesc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bitixxqd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2xosgduux.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2pfrzlqbw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hxnslqlx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bnsrvjyp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2skprkwjw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kosmwhzd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2jubaqirv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rqjmdhhc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2gkqpowmt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcknmdbv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2tkponyrk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2jeydnbju.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwhnexnr.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2gmiivvrs.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lidwecxq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wvjhkppg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wdieggch.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hytveanv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mnneygnv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gezcebth.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zvjbarlt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nmzghzcd.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2xlwrhtpl.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2sguwromf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tzzbouri.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fqbuznpg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vbzpzknn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2crurkhwb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2exbsnbsi.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ilwukzux.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2bgaqlsjj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2gxywpzuw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lseopqvg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2fcqgyrks.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2fybiqozp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2kjglzfda.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2fhrgzpkd.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mheizbwv.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2twzrxaae.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2btbqqxse.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2awfeglan.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2egqypump.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2achnhwch.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2koyrcyiw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2nqyhrrfl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2pkjybfdw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2avlxqknf.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2nnvrgjlv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2mnlpqehw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2xpavmxga.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2aeayeuup.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pcwyebee.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bjtxphby.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2znrsomnh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bcvkdpxz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gicbokdy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jpsfgmfy.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ziwxzvzc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xjhgvdae.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2dyslfisr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2zpkwdhcs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2cjhouafl.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dhopdike.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zurmslef.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxpbnvqn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xqcetlxn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2jwgegbfn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bghxvmqc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lidrpjav.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2evlgurge.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2sjvamfrx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qbcznbcz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jcexnahd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvtbbwsf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2inhqejks.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2jhuignzc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2rxcfimqf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2tkvfkwpo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2dwobwpex.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ajnqpngv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rkgjhtzp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2lglegwjd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2yjqpngld.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ajykvrho.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2bhdlpkas.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mkkisdil.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2tuwrryjd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hosdxllq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ufxrdltw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pstokzov.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2mwsqnqjj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ogurrafr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2nwknepji.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2afterevl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2dkgdmyfh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ynxyoskw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2daayefkx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2esyqxywh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2skfzvwhr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kdqdctfe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2tlqlxvym.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zwivctff.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xksehflg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uobhpxrz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2caaehlwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hiorawkb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ahithiou.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mswqrcmf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2dmjyejdk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rizdoysj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mxukvzkq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eossslus.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2uekbnini.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2okinirha.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ekpbgdxx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2jesezcfd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2jdddbtqx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2fiwiagka.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mlfbvqnt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vzwjzabl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2olthkhbo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jtjznxxb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xiygbawo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ladxpjzc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2totphqsj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ymzarplc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xlmyzfkb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xpetntao.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcgodejx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bposeita.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dsggvuet.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hpnqqnnp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fmqhfhdm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2toxqylst.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ixzyfhui.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2bxcjjeno.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2obomgzyg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qlcuvgcf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2coplmnhb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2lhvhdijq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2doncdjtx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qgzmuxdi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pbujyxaa.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2gfihchfz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wnixamjc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgyxebps.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qnbxfedx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qmwipoxv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tchrgeqg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zihvtbuw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcgphpqv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2eobwkjgp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2zdqaoihs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2occczvqk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqeyscjj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oencqhjz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2urpsmtxc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ufhjxzar.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2dakiwfyl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pxqiyebg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2qmjlwtdc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dsvghewb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2kbefopge.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eghsmyyf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2njyurpmx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2liocxafo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2tlaqibzd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lifaurtr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vjlecdol.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kobsaptu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2bszxalci.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2alcfmmxi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xzowlyrr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mxggbptx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dmuhsmsa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mrganlxr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2cgsfdibn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ogdnjwum.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ieslcvua.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2luvexzev.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dwibnyph.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cdjcvtaz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2riapcquc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pewcuufw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ujhtaqrf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dxmlfpsn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jclnyjrk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xcesgtvv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2oooniinq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uszoipex.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xagsxrph.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zjjmppnu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzzyvyha.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2zbzrbhrq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2kfzsmwof.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2opegvduz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zxofbxim.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tcqlrlel.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rjmodtsi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2iubdqdwk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ihrcdmyg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2peookqxe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2tklhtrau.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qfetxsrb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2shhwbapt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fghnnzpe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2vgdkqkhr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lmuaickg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2muqntyrs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2etymrtep.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rgzdguon.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wlwkjfsp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2bttkwrkn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2nukjmpea.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rpwlakla.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2unnnjdpr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2kuugvmbr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cbtvgspa.html


<!-- 参考信息 -->