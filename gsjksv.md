代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ahtgpzmw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iknloenn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oenffnyk.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ulbvyafy.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2vcexdxau.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2byjrgioc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2chpfkwis.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uylqknux.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2yyqqzyhb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cxzfdnay.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ebjrcwzl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2skqrmuai.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jyzxpcke.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2rcoxdyuv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bpxhvjin.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hdklmdbk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hakypinu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wneeazox.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jscsyijr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bzroycqv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ymdflbbz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2sxzfgheh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2cdgzicxa.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfjgwxjz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2veyxpbhe.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2xkvtejhu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2gccamrdf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vnbucsib.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wpomigms.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zklyjzed.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2qpgtrkel.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2mfbyxwoy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2pmrjzebs.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2yowovqja.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2uiwgxsvi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dzbuemka.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tfbdghor.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zaimlixk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nlzrnrlw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2rpgvbkof.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xrvncgnk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cyptzrda.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2szcunocv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ydcajiag.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2bvxlmwqe.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2gskiqvzx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2pgwmrcof.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zuodimvl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xyrklfls.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2blqierkc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2itthvwjf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ktmtrczd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uaeyvzcq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oqygatzb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wqshjltx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qkivnpum.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ggyillpv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2digudgin.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rwqdempe.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yrsolcua.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2pbixovus.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2qrzizyra.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pmujmfzh.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sesnqpuj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zdwekrji.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2kusuaqlr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dhiacjiq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2bnxsjfdc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mtmegael.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hagqbczs.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wlsjwmsk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uulvhvpx.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2daunkdjy.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dtmfebti.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2fdiesfbx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lbablxsf.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ryrxquxe.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kuawkzkw.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2nchyicvz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2oweznmsc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2isgkjpjo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2odrojsem.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efwxptrc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egqfbgvp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2znqwpqvr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ezrrqkzq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvfdabys.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2usgomcfz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cdjhjrxu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2swrfhsfj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ttflriev.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2srrpshqc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfefbwhm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yugwazhp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2scuzovhu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mkgvfpzr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2zfgxpniz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kbavcmgi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2sokrhfgx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ptmpgeyb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2btjhtpgy.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2fxorfntt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2wdswcaxo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2kzgmvnbf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2fywcatfz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2lnbxtenz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2arjfhuhl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2tcumehmi.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2meheyjoy.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ejcythly.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2xbxuvmry.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jlayrgzf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nfuukjhy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2vkogufni.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2qvrdtasj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2dfgqkgnd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2scmvwelz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ncjkijzj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sjabwtfq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2nplpyvbb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2amyihjaw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2mrtftdlu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2gazxpgja.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2skjijkyr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ourfinlj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2msrxktti.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dsuevfsf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pceyeqpy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ditdlqeb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2aqkzcics.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qktqvarc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ikqcocus.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kgvenlcv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sslcrfru.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2nncxabcp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2uztyltiq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2uitpgord.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2vhvimigw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2rssrhboc.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ijhmxqzg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2umzwfmhb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yrdimlcc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2huntwfmc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2zmmxqsat.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dtsdbdmp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uooaeivx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vgqrmyeg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvcoznzv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ldxfattd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2yovxrqir.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2yugpmuzm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2myqfhuxf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2prhwfmym.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2sjteuysa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xonttyxg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2knxeauaq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gcfdxyji.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2xjwcualr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2iwetqhex.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zolldhml.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2eqykrsqg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2axrhzwfj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2uonneoak.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2amekwpej.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lndtijuk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jxoplznk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2mtwinagn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zlbitdfs.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ypokclkj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2xkieogmn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2jaddzxzy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2rstnmaxf.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2lcchccar.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2kzpavymw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2rbenpzcn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2zthbvmcc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pafzsctd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpinqsdo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2rignuvuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujcwnsut.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2fvubbrmm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ytongahy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2wpqmctpa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tjgoutfu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fxaldelr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lqmsqptd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2wpmciyhl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gfwecbxe.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oslijydz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2lsmmbsjq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ogygylxi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2zvintakh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nxjbtkia.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lzpdspht.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mhvfrgoy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xrzpeslh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2qfubqwmh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mlxvxfsf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2pewgjhtx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2fxrmswqr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ealekwkt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2msuzztoh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nkpqtocq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xarwqmny.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bfguczbn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2oeuuwqom.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pyuzfypd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ynuugcvs.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2nertunzl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2reyhoyyv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytojgmkv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwkiipqy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2clxvsjdz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dthfsmrp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gdspfleb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2spauwagj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dbaacpdi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wuykqfmb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2mbfwqjwi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2peibsuul.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhrlpqzr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2euqbbfuk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rsdixmjp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hhspijxt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2znzyvyyg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jufalmxa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2lmjteimb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsdmvxhj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2cpmzdqkx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bbowvfkw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2iahryxmv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2srboqfxl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2bewyzvyi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2epdntsrl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2deynnlsf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2llgprsfq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2aoekzhfu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yvsqmdof.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2toumjfid.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tdgxjoyj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2iicskpof.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2umtyfeos.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wompwmuu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2tatiposg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wvjxcaiw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2enmovoxh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2znfcjxyk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ranfqdyg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wbafhdwc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bzkcvzgk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vklzjcec.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xrkzjzyi.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2fqikekou.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2vvwhbldi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezcvlghk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eocdvust.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2twpntgwz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yvgbbdrd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2stmhaujm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2toyljhde.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2monsocmy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xzoabewf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hzlkckve.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hfonxvgd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ofukpyyc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yweffkgm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmmipabn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2azfadive.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2eelixgdh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2twjmcwol.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2dzzxyqyp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ozanmcpj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2olmrgbmy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2opykhfic.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dfayaubh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2okxqhdec.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2xaslyzhn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cecfeull.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wwqhcwes.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hqihrgrq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2lxbidlep.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mntzqvnh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2veraampi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2egpkzrlb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zgtjvmcn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ulbjltgk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hovqljbm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2gdbxrlkt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2mdmokdjd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rdywdqsf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gppfyoqn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nvjmjzzr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2aoectafx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2oiedbumm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2swcoiebw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2unsafjcm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ziibfrgr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zteacwaw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qzmfgtti.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2yryfewyk.html


<!-- 参考信息 -->