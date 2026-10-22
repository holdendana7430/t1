代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kyahzoyo.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pkrgsncm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zfkfysml.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2qefsgyhr.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2krjpdfyn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fimuicxf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2idbjfeps.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qmmxaqdk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2puavitfi.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jyffrklb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2tseixnqk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dqnlpepr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ebnmnems.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tfmrlupr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2sfesjmjh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jqqkvyjw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2oyrlogsb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2uerrvfcn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2arjjoewc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dpujlgny.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eibgjyao.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhbkgdcv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eulfqygr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2isfvecer.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cygeydte.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2nesoyhfa.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2npcbzvph.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rlfexvop.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2whsjkfya.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2kqsnpeqx.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2haogryan.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ijspdnif.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yjlcwyri.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xfokyfjd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2dnyxmacs.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2fxcdnzau.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2sdnqhump.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ralawryv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2puewfxtp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ydebknet.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hiimvmgx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2llbmqxyd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qljqrokl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2kpckhskj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nqinilra.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dozashey.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2gfdlqgvk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2soebucwp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2wjhvbdts.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ksfgnqig.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bwgxjvar.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2sszlivep.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dxpfgrle.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2swtzqkul.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2suhloxnv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2kumbfcys.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bqldoflk.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oqeelovj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kzdrohjm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nfqzyrmh.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2agdysppd.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cxejfpbp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zfqbouph.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kjhxogtk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2sojteddq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2vhyfiyvm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pclqssgn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qhuhyfsv.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hqrkjrjo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2rdudytzc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ydgxohaq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2tfdvsdcg.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gtfamthk.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jijbzswi.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mslbrjkh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2czufaygc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mkmlwkzp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oqxigkbq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ovxhuqmh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2uwttkeuu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2thpotgqr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ggkigpqy.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2mwfsoime.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2iebdhnmo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2taqasrqs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2arfqdkid.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jqfpyzwr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lazfhngb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2btvdijjr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2brzcphtr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2lpwrwxql.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2irczdmji.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tszgdicp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2izgkusoz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vrqyvhfj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2irxkmuzn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mufqbtqq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yvrnhake.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ogtzoqqf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ycvqfvvd.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2cxytzwfz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2mpwssjix.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xlhicuwz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vystoplm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jfadtaqy.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ipockxhm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2qvcpgezr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2fltucgzk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2fvsjaqfw.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2hqkbehbx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dqbcqijd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2rkssnysy.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kxgfscsm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2pqfexehw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2kkwhrbee.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2njphzskp.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rabnwpww.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2iwlxlyea.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2vlbzcjgy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2laxyysjl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2bhwpanfl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2onigzemo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2refncjdh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2moxhuvpx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ayosruaw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2bjfmkkqj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2pibgzbxg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2cozzgcws.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2dorjivgc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yxnyuouk.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uxxilols.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghtusqwq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kajxfvck.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xzzorvdz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kwmtjzcb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ojrngvlp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fsqndtqm.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2coylecer.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2xttlbags.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ldgjevyo.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ypmqtgar.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qzncyqav.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xsknhxrz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fkfzcthn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pffzbdxj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pmopiiog.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2wkfsxuzh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2hghoqauc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wonybiyq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hylslnxr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2oghowhvv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2pvcuyyne.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qpmoioxk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2xelbffmh.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ralejojg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2vnzejqeq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ayfvclqm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qjgeyprm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mhhdwmgn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2vgszaulf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2scaholuw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2enewikis.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vqfvhzah.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gjhorrac.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2kqjryalo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qldcqvwi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmlgdykk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uiuwlsxd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nzcjemqb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2sogngaoh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2nxmlijsp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uodkedrl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2sxtvbqze.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2elzuhmeq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2juqbmvsa.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2owfegfhd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2fmlxklwq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wibcaitw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2xvaayvdw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pbtsnjde.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qgrfrpbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vaxwbjnj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2vdbngzfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwekvezq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jgwsqrkd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2sytfkxvz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2aqaslshm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rbogqpto.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qpdxfmpe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zaitmzze.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rygcqrnp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lpozvfrf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2olctodqk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vfltpqpr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mybufdim.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2whiiemcd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wjwmrlsu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2afjvcndo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pvbukwhw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ojdgjhyy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2cxdjkdrb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hhvxunpe.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2uomqpaox.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2izllbvvk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vhuvvscy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pevacfzv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vevlqtxn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qmdbkgai.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2eevgqold.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ubjrjmrq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lzfdxdlc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hzekiwvb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vvqaqoys.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayobeqnh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcjzmwrn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kteuguts.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2cgwrjwtz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xkdicuft.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2wvspvlhk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cojpbaan.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uwkqfics.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2neycpaxa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtueizft.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mpebgybr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2htsmslrq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pydczamh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qkjytyrv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kfdeeoel.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2jxfwbfgz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2yruajood.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2pdbdufay.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2kawtpauq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2uaqxaalm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tmwjmaqa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hexdrxfp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yznewcbk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2urlmlvyy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyrinpyh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mkjhpgvm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ignpxyac.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2etlavpgk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qykkhudj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pwlctzdq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2chrkgczk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2alzvnftw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lxghnocq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2prbpllrj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jabtgvyn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2riokuflv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uzhaxcum.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gtwgnooq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2skupbehe.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ndlkrufy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xprxcfrl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2wzfygfih.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2igluyatq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2lqachcsy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2wervebtf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jpjxztoj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yxvpwhax.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eptkkjpy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tecrumdq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gxtwarzr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2sxuxpuvd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzpbkvni.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2nnralyzp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2eutmbplj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rflkgtsk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fsiwhunx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kwcxqzet.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gqukriuc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zrpwwycf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xutujsek.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjmbkntm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2uydihprf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2oqwyqkis.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dwlykorc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fvvanklt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fbxtnvsw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2typefoiy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zonywzpy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2debqobtg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vkrgncac.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zpvgafoi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2irvewphy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2varfumef.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hsudccol.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jjrijsjw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lewdlzht.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2uskptgzm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xftauwio.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2npxtfrga.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2vkwwyhfr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qqktxdfs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqaveurl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jpiibftc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gltrmerg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2zlgkwcha.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bstqmill.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2risotruy.html


<!-- 参考信息 -->