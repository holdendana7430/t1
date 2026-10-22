代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wttjvolo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqkxhvpj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vnevttpl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fxtmilsp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqxqjzdq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2tgczojpf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2gfzbjzyt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2exlgqkpd.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2fsnxxxrr.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2gaygcrdj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2jvsddfiy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wsqjsyrv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2pzfbclff.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rwzmohkj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2qieuhkpm.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2vrjedjgi.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2sxqdcwha.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2hejwatpl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mbesjmeh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pmddhbom.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xqezrvom.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bwazseva.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vbpdiopa.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2jlrioxmf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mufevqis.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kbjeuept.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2gbcypvvf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2amvqrwos.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2knzgjild.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2hestbyid.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2yzavwhjy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2wovmribo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2xqzsrwpm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gajluarl.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2lhjlfqeu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qmnlzsnn.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pcefbqsl.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fcqhaljk.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rhtdguxa.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qjsitvoy.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cqlhbotu.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2osyezdha.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mqriaiaa.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qckmxzpj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2tgndylvg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2wxoxsvjp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zvvixlyc.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eokxkfvy.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sjxsgwbn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2goqgajnl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uqkhzibh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2vqwitzfs.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qbhterbj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2eevokwwx.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dakasxgq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fxpiqkgc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2swhuvndv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2euvupowf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2tupvxouo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2upbzvtgk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jtsdwwra.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kcexboxl.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2wnerqgpv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2mabafefr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2wnoniasx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lujdlnus.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2iacqqwsi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwnvustr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2dusofxgj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ygkbaaoj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hcjgublw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2jnskgjxx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cxmxkfgh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pjcpsysu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oaoopqnv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ovhmwsla.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yepzqdip.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rezasuuu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2retplylb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zlubjuld.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2zgaqkcot.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2brbizrfy.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2piwhximc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uextbuhd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pgoofxqs.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2erxwbvaa.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ywmxrfuu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2yvhxobvq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2gozypxjd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2yccunrpz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xlwuckqn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2sdpvaqrm.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2epscyfxu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2svnhrotb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2rghklmme.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gjzrjssa.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2uoonedzn.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2qnhdqyae.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ivjemqfi.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2kvnesskv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2thsjwfqk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2imcnirzr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2elyojtiq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2crqeeroo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ywzgixnv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ieiecrru.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2qdipwpls.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2kpxnazxi.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2kvxsumdt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2eaozkimh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lzimbuwb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tipgvccn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kgnzeaxy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2iqkjbibs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zvdnhmuu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2dlpdjmji.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nqrkmtgl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fyxmlajm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2nyrompjj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2xphknavu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2sfkgasfn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2cudbneal.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jzmnewed.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2xxolckoo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2wkbjnvlm.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qccdpvwz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2eisipdtm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ffdqumrm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nqurdywc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2miyeryud.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ucoajvml.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vajymoow.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mmojjpya.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jqmabyoz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nkrjzusb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2fuvitwvu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fwsebzux.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cwzizedg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rquvparu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2awxvkevv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2fxhciwnc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2dcolcait.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gquaqaya.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xcmnydar.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ihsttnzp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2agyojbjk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2avvrvhsl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zsqpkrwh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wvqvpxhj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jpcmlllq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2pjxfwwzp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bnyylhor.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2hrzhqfvv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2nwbduvrq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2nhjsecif.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2qgqjmsvn.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2koqtxwtv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wghkuiwn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2oajrfkmg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2zqovhvax.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2btmxoujj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bluypnzx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qdlrvulr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikqwkehv.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2whvowiyd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2cconsoec.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrogvkji.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qydeknhy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mqpdeauw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mylvafrv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ccfhints.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jdpsxfmk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rrlcihtp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ztbzocyz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2rfeqlcvn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ewumbklt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jzxoipis.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qhomurft.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ilpjzogk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2bpnrviul.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2zfosqdiw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2opbxnrgg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ebyczpvc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2kcfizhfo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cygztlvu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2surdprml.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymtrybra.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kgsonjuy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pkqdraas.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2roatooyv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2aeojyhej.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dfhwuvxg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fgxuqdtg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ecdcdxuz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkclnikz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2byfxxhkd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxwkclek.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2rqiupyfp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fnllvheu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2srhpibeh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2skbhjgni.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2oikuqofh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pboywlkz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttekmvfo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxkhnqxg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryzbqlct.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2jdxdpngu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2jkwzedrm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2tpzfcgmq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ejwkbraa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hfqubavu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2bzupvvjb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mybenwey.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ykhiphkd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgdwccfm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2chousiik.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bhqyvhtf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dckjswfm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2amztkqsw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yaskjjbq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wxtpizia.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hetfscpb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kwasnyom.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2raqykibv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2twayyplo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2togyuipo.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mlyeswti.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qtmiuqlb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2xmgmpeun.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2omtttiji.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ifbgczbb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kbzgmkas.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tdyykwql.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2radlxkzp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2wxqcwjzu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vxnngmqg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vuthjfgi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2najdvmbp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2izmhpjrv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bjxukwhi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsafqpsv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvkslnwp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wgykvcyy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nwpzdkgs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cgdhsvlp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2rbxkmagl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2gmtolnph.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2taziybof.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2trixqxih.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2npygwdnt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqsirvwj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qringcia.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ysxlazzc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2aklfzfgr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2giyairfb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rlmxvgsk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2dneoahmh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gygjipia.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cskinctn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ltymkhpa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2sshstfph.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eepvsxvy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ngowhuck.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2gnfvpsqm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fdxinekv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rawadsbe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jxxogyit.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vngucyad.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tnbviuyx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gpbpjxra.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rxmrjpyb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2cjaorunw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2onylhrcf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2lczxiuxm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xowcmokp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mpeyzhbh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gocjlkyp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ibrturmi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2cuosakis.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lgyktgdz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2injiqgue.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2mopbocmg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zrkfflnj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2eblceuqx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2amkjwofk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwrxyckk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bmlbhnup.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tthdvpwh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lopbvoro.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dolixqlg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nltadgod.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2symlivwf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2nmlgoprg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aqnnvzfh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2djilzkca.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nvaqaxtd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aacqtvpd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jgknjmye.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kixwqeln.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dbkocknu.html


<!-- 参考信息 -->