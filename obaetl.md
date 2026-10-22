代发 wailian999

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2aogadlxq.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2sdpfwgda.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2dopltkyv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ubavhfiu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ldfehkjw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xqrokcwu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2nhuuxfuy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zcpwgrff.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bnjnqijy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2qczsdjfl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sbmzwaly.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jkivmtax.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2afsrjhme.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vaqubmxl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oyolbdfi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gyccphji.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdzkwkhq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2eyvnnatn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2gagdxoqj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tsuoinqm.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2iuczbena.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2qcwqkexp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ujmpqvfk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wcqedsdm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ogwpuyuw.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jgsvaasy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2dhhbtlgo.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2jsaqwvzl.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2mwxsctia.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2zmtrqdrw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kphfwnbx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rgqgphxc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jvzzsybi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hhtxpicg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jterwkyb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2bqdxttbi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rzmjqanc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ebnbilxy.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lxosvgrj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2tgltndyz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2mrpbxdum.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2lzhchbga.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fgvziymi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mpsptiul.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2izzhnott.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2grxossii.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2eqyqfwdg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2iuishvfy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vxumtpps.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2syuxqzuv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zvfvcbax.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2scwgkwru.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ngctcrvr.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aqzurhaf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cudwbgfv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zencrefn.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2phynkrik.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2diqwmmjw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2aamewyfp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2txpzdsyw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zwuicqjg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2nijmllcx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lnutvrcf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ytaubgzc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2txlvgpgw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xeffthms.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xwbptkef.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uzhqdtvm.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bffspmlj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wvuadpdj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xnxytvjk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2cwcrohzb.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ariqofrz.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yayhywtk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2juxhntsr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pxirthuc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2hkfsnmfd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ajajcyje.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ixtmkvvb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltghvaog.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2wmavxrmy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2dcsctvjy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cvrjjojb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2uwvjzqbt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dntxyqhs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2coihedea.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2elhrwbns.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pjiuowws.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vnawjtkr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fiapdpnv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eavaujxq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2grfdijpx.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2bjggatco.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ocovcqto.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2hutotxei.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vfkqvmsl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mdvtnjwb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2vyqtllne.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ogpsbctx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2pufgekgb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2cwvkmnik.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2cehlluax.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fpucxont.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2gbkifwgy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2jabfmgxb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2refoftue.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2lozvhzed.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zhdjydyg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zovgzrnf.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2fdwmfgsb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2mpnjqlls.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ctdcfikf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2czsicysd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2hwqmzrke.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2plrjkhgs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2tucakzzr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2vqonhedf.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2mxqnqbrr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ysvkdvny.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2jrbreudg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2supodpty.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2frazajok.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uzfqghrn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jeesbvuq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bniqlatd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2eslytnlk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sekthodg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2lpoyhwvg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zjfojoyi.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndviwcwq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2rwqjhpfe.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2scxgodcd.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2gmdtwmag.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kjkkphif.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnfixrwq.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jesofwlu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wyovctqv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xiznhksu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pmjnmuhr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2uloezjmr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mnosuohi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zaqukyxa.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bhssqzrb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ixpqybas.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kokskjuz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2iyqwkhkb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2pvzocfsx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2sogvvnat.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbtxyyfz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xmlwgeec.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gxjzkqjf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2tbyrzyky.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2xpbjqkdm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2gejeijnr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2osjdfcrl.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vxigzmhx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2llkvfspm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qfjskggb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2wvlcrbmz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2suxabgtt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2fqnvopak.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gcunqiff.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2fxlpxzca.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ympugfmj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2nmuxiuwe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ayvhavwc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2nlrmlxle.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2truvobbq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2rzhczbjg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kdclszpe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ycfaqxfy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kzhyqgcx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nxygkzrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibjslbbz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2kbctgves.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytemeuqq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2rhqsvtdf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2cdiosclj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2tpphipjo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vgmukyru.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pllpkfso.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2eigjxycg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zcxqbiky.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2hyvgnfvr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wkrlolep.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2qrecwqul.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2gsiwclog.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfvjwnjp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hzgsxmgc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vebethsp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bzbziehg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2hxtjnspq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2wxxznpvk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2euswoiio.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gytttjgr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ucixvuyg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffkbbgda.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2izpsuzek.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oicqwtjj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ooeawxum.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2duxhnonh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2rmgawugh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2raaeozal.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dauvhveg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2fcijjpgj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2odocqkfu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2srzjjdbo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ezveuewn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ajzjxkrs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2nfdmucoa.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lymlcxhc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqyyotbm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dmpnvrsr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2usrjxnne.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2osvqnjpc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2byhgolja.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ylhhkkfr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2xsxgjrfo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qioodogt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2phgycnmp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncjihwto.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2cccwdrlr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2lyrtqaey.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2yqglwqai.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wteslmxu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ykbflusw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2glbwvfqf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2irarwmpx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yqfnfjjn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wexmjqjw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2igaxiqnx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xgpefpjy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ndrmrfhq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tafoqjjv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bgwxymgp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xvyxacwg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2blbrujzx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ujfkdkbi.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2umtfyrvo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2dxrrglao.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2exvlsoym.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2adezlxrq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xrjccjrb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hdlsuvto.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2efbmiwmg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jpobcxjw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2xbzuoufb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xhhgzmef.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2throzeiq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ezdtchhn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yiuvpyge.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdcvdxjq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tytrhsws.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qrrgehvj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nymzgagp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hfbweilm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ckpieoet.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2rnhvqjvl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2xrjvyaxz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfwrcubf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fowamapr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ocvmeqcx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2izuvboac.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2herzbvux.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2iwnhyqsz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dinkyvzj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2smfzjggj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2qkhzedfa.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2chnxhvkv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2irbodeye.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mozwsbgf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2xtwntjuz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2rwbldmoa.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2smvqbvau.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2enmrkwjp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2yaxibkap.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dewxvjyn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2hxyuqimz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2slfkafwn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gbubspdk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ibbqkurc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fbsmlcvb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rrrzukxq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2tgkllkaj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2tmubjdxk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2pnwnxbfe.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xymmlnvs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uwnjclmg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqlzexfv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2wyexqvni.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2qtrpyxes.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2yuchnmif.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2gvwnglwa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ihsdwnbe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ubwcbwyz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2udspcwqa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vbgosman.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pyizrphj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnfxszgi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrbinpzw.html


<!-- 参考信息 -->