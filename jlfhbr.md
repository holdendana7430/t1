代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wjdxextn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2opuqfwas.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gsjwlseh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2knrzsfsk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wbuyvztz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2hzfqasrw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2smyazuno.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xacwlrqn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2zwcrpeuk.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2hkoeylvz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2iklbpmkg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ebbobuwd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yegbdfsk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kkxdemww.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2tusqlzrx.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2spilvcdp.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2olatdouf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2faunkljf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2flitntbc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oquayebg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2noittvyg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wdwutnty.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mpdpckws.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2nddatlyg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hfjzhsqy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jwmgtnur.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qiztuetu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2etfwqdxr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2wsrdwasl.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hbofmbvh.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vgnmgqaq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2nwgtmlyt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2qggwaupi.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ldynivlu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ubhbqxvj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2anatooui.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lwtemmvq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2debuuevi.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fjckxcrj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2spuobyiz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cimrjaae.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ztmggfud.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lkllllqv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jyqydaql.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ljargjhm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2izibqexk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2crasznpf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qrmecnni.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ixvfxrym.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2nkiwgmyu.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yslsdpww.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2azkytxtk.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zvzmktoh.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dkbzbkqg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nkynufjt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ehlcsvug.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vvmlyejl.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fsooeveo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2tckcdgvj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2noyuzuaa.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tbkjutri.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2owhqhfku.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2nzmnmeep.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2tsbvaoam.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2oiyccxox.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2tkgrfmsb.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2clzmcgwk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rckwmztn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2rdytwatj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2wqrxcoca.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ubznmivd.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tyntdbus.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ayjqltfx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2csdxcnvp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2juzplvzg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dvolvlcd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yslrcewa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2utzvtmyq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ahozebcv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2avywtdla.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2auhvyokw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rtcmdvcp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tjlxzucv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2bwvuzmfm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ugvjeuni.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2wergagxj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ocngnqaw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2lkdbemlw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2uhfsmfev.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2takyhygm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2igttqlto.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2aesqfqfd.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ljxrvskz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fssyeccc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2zyoxreqm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wwbernlv.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2avcguuzo.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2xrgxfgly.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2fnsrtmyp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ekzkletb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2xrwfbllt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2uzqxrmxg.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2vwutuzmb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2gxngxetr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xpcejrnp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ibotdnko.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2vqzzggil.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2wauuvfkl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2leghxyuh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bznocwmv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2beqlooxq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dxfxnnxw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fpumfkzx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ifrgprvt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lgodhijr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2krgptvvi.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sqtycizz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rghrjwwp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2iswjudda.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2easysewi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ffawflow.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2iilcvebu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2upswahkj.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ajhwysxk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2eyhctcnq.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fxyvkbzh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2isosjsiw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwiwwohe.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vgqgvlnf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ikdecgmv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xqenntlx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2klluuund.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hzlwafso.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ezjtxgha.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2kwmtcaxv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2iipgrdyp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kniuoltk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jiciotmt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2knmchvyu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2hyediepo.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2dokzashc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2xsuvbvqh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ukvcwhit.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ozfbptxf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2pzijtfsa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2otrofzrv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ykxlnbmm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vpqacytn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xinilzpy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kfclysbg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2aoqkzxlx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2dpytqizf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ufheggwr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2vzblytkg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wgwxjbja.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ucoarxyg.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2nlwcbipn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2dmyrazxi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2mjvtecph.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2qgexpqso.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2apyibnwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2niplqqbh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2nxitifhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzybbyxr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2gjgyodib.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2mjsuqaax.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2emcnbulr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2aasqmzyo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gfnjekav.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jvpjowqb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gimzktgz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kgwsrjag.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bfzcoonk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2iotuezan.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2hhjutwhp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2glgatnyf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sbrjmezw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vypsyknk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2diuxppvr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2pcfvqaid.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nhsiejzr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wbuqxsyu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2limdedcl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2hjkepvwl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pylzwmzv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qoxsmwso.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2eleslbia.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebyfymfz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2atcudisr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wtwewtrc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vaawyior.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tyctlhpv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2tunymcuf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2qyjqhtir.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmnskbix.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bhbgthvi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvnbiucx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2jlqiynmg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2szfjwklz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmiemtma.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vubbdjni.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ppmeiweb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2xfrlkeaz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdogcnij.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gaucprev.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlfaemki.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ekcgcpzi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ssgmycgi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2kgivaaap.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2cfaiqgck.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2eichlhwf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcankdsj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncpxbjwa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rplnaraa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2asondgwf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qsdjnwxm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2mvidhsid.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2okiyfltm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2fslzbiyx.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2nemboyly.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wluiungd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrduiuyj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bnlbjrjr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvracnlf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2kznkpgym.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2eyarluzg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrqkidvy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rnwkevff.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2gwcyeetk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lmylozhb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fsmredjv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wnqouoij.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2natcuhdo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mwzreozx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2hyizkitb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oijmyosk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2wijuceri.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ynrirblh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eoocgrdc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dgwnuqdt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2amrrswip.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrxpvuzd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mybzdzze.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2czrluamr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaojnshw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2zcyjomty.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ytnmxprq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2argbrkys.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ifejerhd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xcvaqgnb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2pxkpacnp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ygdkadup.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2aatssovy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqydlmrh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ravqyhoj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ubicouud.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2bqexxsbi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2sztekabt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2czkhrzws.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sddgodkv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ueaokidy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zjkyqkyh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qzrcopnw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lipdsypu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dfzcxmnt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2qujyjqxb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2plcqjxgi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xelnggjt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jmnmndgc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2dlfvddnw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rgehssof.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2sdnbfkzm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2urmgwfxp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2owrvrdxf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rozsbntg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hyqwjnwk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2csnilldp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2hjaljzia.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ctngrwiq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2rxrmorlq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2gcvrhbdf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yzylwima.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2vysegozx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2kkukjtnm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2smuynhet.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wbwmfcvt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jslqozwe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2xpkywlaa.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2klsztflr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jnluxsee.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2oxmrqvzk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2whwoxewq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2upnthatq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qmpscgbl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ejvhevqq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2unbffsbo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jwvoavlz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aocdrxxp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bcswooiw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ybcfqfpx.html


<!-- 参考信息 -->