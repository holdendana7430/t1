代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dvcbrqbm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xyvdlqyj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ktlsfwjv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2lmrgrqnu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2podgyntk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2lznqflgy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2pkesuhdy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qbqtcewu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uchfdwvm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bglfrtwk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ljziscgo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2pxyctmwo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ttmksbov.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bxnecwjb.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2eanrzwpm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2twhggvpu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2mqbvglmc.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zvapugpl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2owwnuktg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2nrycqmbx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2emnzztuj.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2qrevzdvp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2dyorptdm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2gptvlbrf.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lxscitvr.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vyglqfsv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qtxqdumk.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vggaoqpv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2olsgjrhx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2apjtxksv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fbsaamup.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ktfumevb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2cjjngold.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2yhrdagvu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fpzloxva.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mrfqbvsv.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jkvrjnmn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2bbmhcvor.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vcmvzmcv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2nvwcaqxa.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2owleonth.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wltksnzj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fmdottil.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2okveqeov.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bhsaekmg.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oucryulc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2rjybirbq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2zvscwdyn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vgoxquyu.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xhzbwhko.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2sxyisstw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tqdorgkw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2rpdlejfy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2aixlaavg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2gygpyehs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2mnuifyvw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2polvdzbh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2cybmjjjg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2trfqxeio.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2nhehucrl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zdxrnfqt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rsswfgum.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kugifzdn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2unluieoa.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lwvritvg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2npkmsnjg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hsumbaww.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hmribpfx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2tlycxflq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xngbohno.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wfkzdjsg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rexdvhut.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ehncdscz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2punatrgg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2hcopumqg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2oskkskug.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2glanwqgy.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2rfelnsfu.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yhjtqifb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ncnoxgow.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ywcqsnbu.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jkbqgiob.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2clzcoksq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hcbwqzmd.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fiqpdsjw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2gczfyukx.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ukyefidj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2kleuobpr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2yydvcrju.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2brqownej.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2eaxmggjl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2dqzaixpl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ygsfxnue.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2dqizjyxm.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2rlqjemsk.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2jrojqcmt.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zoldmpua.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tjnuxuts.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wprcycqf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jtgsicto.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qneqwsod.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2aizzufzk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2oqlehmrz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2otjmnxfg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qxczyrzc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2szjscmlo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ixkabgln.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ialganrt.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ytehxybx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wigvomlm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xbmrcvwy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2jhqwglyc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2enybbmde.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pgyrjrqj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2nrolayoa.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2seawcykf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jagnreha.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hgfnnvnd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hcyewuei.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wyandpbb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zuihynpo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2efbvorag.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2vgvxflkn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2rgjkogbu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdtpdozm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2foumiric.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tyowsvjd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2gacapfuv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mqfcmgub.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2clwcfqrl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rwxcgxyf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mfgznoxw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2umqbmczk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tjfoerim.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kzuhbjoq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rftnztpp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2thcexohf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2aznfvuxb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fzkvjxvk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mkmeblav.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2eebznpur.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2defqrtgz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ffrmsibw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2dyqwppcw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2yxfkidjx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2geqpuutr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2hafxuvzh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ddwwfppj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mfvkzkby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvhxfqwe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2smterizo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhqxtefi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2turbttvo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ksztobie.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2xuanqlyp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2odwpcpzj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pmhvymce.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bvrjepvg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2dgygxuue.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2adzbiliy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mpcladah.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2iiqemitj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xybompef.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2unigtqwk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hhxyheka.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fslgrjco.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dtqgbiiu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2liuhztto.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2lijxansx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fcgsrftm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ijykggzx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2fzxeksgd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2saljvkxh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jngbisjc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxkscofi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dscpzkia.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ufdugktr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2oftsgrfw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2akyenzns.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2flcgpfsn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2elsnnckh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubsfwhwg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2praouevw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pzgtiqzp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rurihody.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2hbqurbql.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ikaviwdd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2lurhnuel.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cbmfyfpr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ddvyvtlq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2dplqbogb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ykttfgly.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kftrnies.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryyyvqup.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xhubusrr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2jhdlteuz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxvgljcm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2fgtzmtlq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2bxfutiul.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2fummphrd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qtcdryxv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ymsidddk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2guvqjscx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2doameobs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2mahpawnx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2htlufhnf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2inxzpdqt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2jpbqytwe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmppsxgc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjftosbr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qljwucic.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2afyaviie.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2zyrtdofc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2siequsny.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ktlvctyq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2nbykeiaf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zqpuwlef.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2peovlstc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dnfgcoae.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fidtugkx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tbvtzekj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qfqtspxm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2lwdflkuu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xcgffhav.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2swoolybp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hqjhtsho.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cfagnqdg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiutdijm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2juhycgpq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eirncdov.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pcmbgaxy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2vnsxcdop.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbvjvxia.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2yrmftrkd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2rlsmwuay.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2qdcwiuga.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2eajedbws.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rbtpechg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctsydhzd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2mjchsqyt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2iostpntq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ggqmjgbn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2tggoeygd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2owlcxlfy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zadhjzqv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vcrowlub.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fsufmywk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dquxpvog.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2skajzipm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lgeugyqu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nihuwxui.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2tlkryedu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gruvqvli.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mgozrkne.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zuxptsza.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2msoninfc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2eidnfuas.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2fjicwuzh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ivdvoxsa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2pmbnepyb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2tsjlwyys.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qowqrkea.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2njwnbztx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bxfkwlul.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkhlqpaj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2phkatzdy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2crdankjf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2sypspspq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dwzmxgeq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2aijikvjo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zczbiuar.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nnoeiqdx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjxcaswf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnuqhiot.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvohnjlt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ysysqija.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kikqsyuq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2enmdmqsr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2xktlginj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2jcefwuth.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2euadaesw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rszxmjkb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iqnkrcvk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mivcaszl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qmfwgvet.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rexgampk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nwfdjklm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fcmcmtma.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vzodgtly.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxxabwmf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2awrxofyn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2skaaanzh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2texxudyn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2mamwvizc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2kytisjoq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jhydfruh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwtcylgm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bxudvgtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdkzriyz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2punkbtnj.html


<!-- 参考信息 -->