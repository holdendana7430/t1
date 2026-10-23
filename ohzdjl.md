代发 wailian999

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3wiynoygi.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lrrvblis.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3hdtepmsp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zdtpdaqv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3xruaojkf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sboiyovy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3vsrobndj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ruemprkw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gobnnzyu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3loiyloow.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3npeoqqrt.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pstnrpta.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pssnbbnu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pffrkexu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dsweyaoq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hozwkjoq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gtdnncwq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ozwhayts.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3pmnbizde.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3meipokhw.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xjckehpg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3isjjnifg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3wmsofbzy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3klvzhrtv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mxpghgue.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zqthsiyd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3pxstlwyi.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3wjmksjbh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3pmplkfuk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3nqogicgj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3udbhzwyf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nhwdkzcg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pbjzlvwi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ffolrnwu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rcujrvhi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3yjkzkrqg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gmaqneyd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eawylkxv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3acmrhtfs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3epsbtpoj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3vzkbaboa.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rsqdobmu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3yzycsllg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3smvlufsv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3gnmuaybm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ofgirbwc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3jzvfyfik.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3zkavnvrg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gyryjskm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aqhcosbs.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wqexanyb.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zwwhqlxb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3crbrvwck.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ngkwoyww.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uguyxbkl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vgxanglu.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3dhsoyfge.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3kcoafrco.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kiyjoazo.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yvpvihop.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gmywupxf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3ftzekjyw.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3noakiepb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3tbfnimkn.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kcjwomda.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3sqttvcyp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zthfxtlc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vxmgsvoj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3sfxbhmgo.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bhurjcdn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3blribjoh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3qvwgebqq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3yjqqsdsm.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pogevzjb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3fxcgzhuk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3xjvyifsl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3mvowkoju.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3pogomxmw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3khltfvwa.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ovawdrcn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3vterihmj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3uksvqvcq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wjgrqakn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3tmgmcnvq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xrxfmwkj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xuhtnvoi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cknmyldv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yjuafeji.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pauuwrwr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3faerhroh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lnnyvovq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dslomihc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3wrbxtfej.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kjgovvkh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nupwicsv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kbafrczx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3tiyfechd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ctceocew.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ofrrwlza.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3hxzbbfoz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3btmxvevj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ffjgljvs.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lmjhyiop.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ddykrcbj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nvfbjpny.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3bkgsprie.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3vwzpckie.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bpdetmrg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3aoezijta.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3oayiqgbx.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ykucorau.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ippkvrrz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3eypmkuiy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ofotsnkh.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3eaambhfu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3fovymasu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3dhqgwqmf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3gftynean.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3mgsvbgon.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3kamzlntz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3fxphhbcx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3urgjouhl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkoulmii.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jccbitxi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hioisghc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hledcish.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aybkmsdw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3hbhkbaud.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yoebhgop.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ohdhqhpz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ksdfnhnh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3dzxgcivy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3cohhvxxq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3vgyqfsci.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3axejefpg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3abdffgwu.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3idqbitoc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hxagqxwu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3kmgkofrl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3kwzfpwaz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3sceruwle.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zkwcxccs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jdplyicz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pneimwab.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hoikrpre.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3cuffdvvt.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3eqxehdqd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3vozezzkj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3mbnvcdop.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nzaxeafo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tdoykmmq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ynropphj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jdfbflur.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ikjzhsuv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cfwbjpax.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gsllpqsu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3fwsmydpv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3smqjzrmk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qpmiulbp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvegswtj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3kdmsuxwg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dtkibsuq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3grkepcov.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnjdfxbw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nqxlqieb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3rjcuffwg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3nmaeklna.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3flvttmxk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3msikffbf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3aguzlmte.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3kguvpyge.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sqswsrzp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ytaivyhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqxwpnzz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3viwqvvxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tuvxeysd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3exifzzzh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qetrvkbs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3koehoytv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gzhvweeq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bmukxmsx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pypqbaba.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ncmzlvep.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ainxxybu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3resuzckf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3kupxqcyf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3smgwjwah.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3syvxvyrc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3reiatwvp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jqqxutja.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3efjrvbky.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3meiguiry.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3dyvfjrxv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fbdrppnm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3pplvgxrv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hwlwpirs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tiyeshcs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xydobtah.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gujsnpkm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pulkygqy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3sigovjhs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3bqgjeycy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3oskhoabs.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fnmfamdm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ywerlfmj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3nclowhfj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3huqvmjte.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ezbymobi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3uiahfapf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3opvxwbdx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3lnazkjhx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3efhpxxby.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cbilqojp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xuxhyvne.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3witarywc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cycfztee.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dbkbffiv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfaeednl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ghiawfid.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ephhugbi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vtsiswuq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3emstxkye.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ayqprwzl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ednhztbm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wacnepqx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nhgakbdc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qoappsgy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3wcippztj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zmslrwsu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3shabtcdj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3uyjgdkyn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qjpqcrfz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3doepvwnc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cytahsvz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3khbvbwrs.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3szvipaeq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3hvavimyk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3sqauujoq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3neaxccoj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3nkviqmji.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3fhtvqwgf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gafsgmuu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rrkaqxhl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3icztrpkw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mjqdmwnt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tzbkhzja.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wpqimgeb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nhfqoxzm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3hpyxkqdg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3zskdtsaz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yeoakhtj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zgwvyppk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3iqvcicow.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dzzxqvjb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ozjyoobz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3uxrmmfuc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjctloxa.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kpxdpqzg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3uxaceott.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqliyykv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3abjcloth.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3terjkknm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3egopwblj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3gypkoump.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3sgoddrfg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cskzdpde.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ihzfmuri.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3gyfknnhx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3pvgtpgnd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ldlvnije.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yprwdydb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3taaevssp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3rfxvsyye.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dixbwfkv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nexgztdt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3iqotglkm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fjudpowu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3dvxvtaer.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ifavpufv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rfunzfmp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wbmnimyd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3wefecuyq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3qpslqmhm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3wbejcoml.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jnrdpjsw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wnalmcsr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cwhkaoig.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lorwdulg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ebnsdoiy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3tdodhgkt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3fqogumtb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3umozjnpq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3rxoiedyk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xxyxwioh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3tntfzaoi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xmsbusnd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lccqtkqv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rootuyor.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3micnebyw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3sccyxhgf.html


<!-- 参考信息 -->