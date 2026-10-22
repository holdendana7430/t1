代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fscmmcmc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2rdxtbeif.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2lqqaqwva.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mfuqrgvh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ozdmwzil.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2shmyqqab.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2mpjrbnfl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zluadbsi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjwtpdkz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yvskpsim.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2mudvspuq.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2watfoehi.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2imipxjvi.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2sppsulck.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2myecqpmh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ytgmwtbl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jtrzcxzp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fovkndtk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lpcheqcm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2grzntwiv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2roydovnc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jfurielt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2iaxqwdah.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2qpixumug.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2cutvsyxk.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xocdtnzr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vwnbheak.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2xlptlvps.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2nrqsaizy.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2tyorcjnv.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2twovswhf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2vnjdkuhb.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qnwdvmmg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2llwcrftz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ypcgoaos.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oznpmmbw.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lhxuhpjp.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2myyclabt.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2caikxjdc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bzjabtmc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2fhdrvral.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ugbnptnj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2abjrzpwd.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yqbqmpwh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zoulgqfd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2pgauwfqd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cssonkqv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qribffhd.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jymnfdmw.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2lshvfeqb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fsmstktr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2daqsqhag.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2navdnceo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zkuiluwi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2twhadtcu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2cszdhzvj.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zadxmqtf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pmjipegn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2irrmpwpn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2djwevbkh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2mulrlwld.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2zonawrgd.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2cubinpzc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ufiexouz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2gbjalhur.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2jrnewdoq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2easddmgs.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2llwfcqwm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ufbjwanz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yzntvcvu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2skfamsbr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gaopxdmz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qmicpwrb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zwazrkdp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2buirymth.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ffhkkqgy.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2znoacgwy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2fakelofh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2copobjug.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2razwirog.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2cjghykzc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2lgaevdho.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2nloqoypt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2dzplvsgo.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2osdhugts.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ncmpyjdu.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cgxlfbgi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2vaaydpvs.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2yyglxsnk.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2sjatbqad.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2igpjynud.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tyylozcp.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2basmggyv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2rqmstdgo.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2hadaturu.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2bzteshvg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ziqqprzx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2sfvhhniw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2kbqtztag.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ssslurzj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ebleksxg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2lcooktsh.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2qyfucfpb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2earlbtbo.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2mxbmfepv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2atsadmdc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2skvinuep.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tuuayamx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hhlcpvhz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mxjqezff.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lbztlkxj.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2kxpmmtfj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qvnomxyp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vygpjoss.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2rnmnnsso.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2amppcajj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2xlgfcrvv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zsxzylhu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijfglhbp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2eykqhsnj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ignwzeqh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lnkarapx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2irngcfcy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgpquxzf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2aggkwkap.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bkryzntk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ipxflkgk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2iwkxwgbn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jnoduuxa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2anjrtqcd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2fcfqwabj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2uckibunq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pyadapnd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rhdnivvu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2erykjnxk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2xbmoqhba.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rpmhlguv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2yxbypahn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2igoupzef.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nenmylns.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xlhbtjny.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2fxzgvjjm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmbjrlfe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vctchugk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wevsxlcx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hpklybsp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ruqkrsjj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ektjxyah.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2qvrxwgmf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2dbyvgqcd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2lmlxqbze.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2vfojsxvz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2mjvupkaz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tyumyowm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2fspojlns.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qteacpkh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hskrlfmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmqzppcv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ugdutlsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdtyoktu.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2cgbsyjrn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2szgenqnu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2mhmaacyh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jgfhcpvs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cgfwdsqh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2souxvhoi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2comxufni.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mxgtqhmf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gcontgtq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2dkdyapai.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2oqgesnkr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xayhiscv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tdhwstba.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pshpumew.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2grsdjbjk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mutyktpg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nzutfqyj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zbxhrcuh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2acytxhfo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2dimmpgdm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tthslomj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaskkcyr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fawjncqz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kslxxlsq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2maeyrhgr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2pwdyjryw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bkyssqex.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dsfsajpq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vwgittmh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2aabahazz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2quyyaozy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cocoptqp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2unadocly.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2aqrphbiu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lehywrnx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2hihrofej.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wqjpcqpe.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2pcaxielt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2antzvwfx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2odyvqkdt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bgejvjjt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hsukdprk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2tddpsqcb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2zuaecuhr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2czdouyar.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ngqdzvfs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2kbcxibkc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrntnxse.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lhguyxvm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrbqptyq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rspfombv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2fchvzjmm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kwpybyog.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kizorsms.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2friewynt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2npvgflyq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrvexsgg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xekyqzur.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2byvmyofw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wivpvinu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2bzdaonub.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2yyytrass.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2normylll.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2pregshxj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2dmyxmqdv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lsfxcgyq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ngsbxtkf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ejncbloe.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xrrlbuqi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2quvbtxqu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rbltaddj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mdpkybco.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wukqosde.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hgmvbcxp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjfyjbmr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdtmueky.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eclcvkvr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2teubqwxu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2aqhjgtyc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2sycsyxev.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgsfweiy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2satgraeb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2gdnedanj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2azqtksyh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dwqhwomn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2flymbyra.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsrsgcsr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bnodhuod.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vexrsmwc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vkcbfkiu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2bhxutarr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ejhfcfcv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2sqfiiqnu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2evfagbbs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2svhauneo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eatwthlx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jejcexjk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2utjrxemu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vtqjldsz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wvpsmxmn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2qbrlcebf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2wxrweowy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nrwbexpb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bqmeougp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tboqammg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2pwsqgunu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2asqeurmq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2dsgmdvuq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2jrlfqgkv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2dgntexxw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2odivschz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nmvdesjj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2unckkrzc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2yafuiozh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2jenthlvf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vbjufdzb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2kxzymplo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2izgkjfqd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2aztfxsmp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ddoqdxqm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pobtldqb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rmiypnjs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gzvulelj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ulpxvsmf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ffzgiwxg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jshtxbqu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ycobrmme.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2lhrmxdil.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ivkfvliz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qdryfnxo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iucdrwum.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jyxyemrq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hmvvgrst.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2clgtuzan.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2onirobht.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2zezbemei.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2qsppdhge.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdbmrwwj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2honnmfdv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cscwccpq.html


<!-- 参考信息 -->