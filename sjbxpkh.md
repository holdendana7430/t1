代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.zdbjq.cn/Article/details/grfaycmgr.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gmgxurkam.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gugaxusxj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/guqaskiqe.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fehbvm.com/Article/details/gmxvshvaq.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/grghaspio.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gqipvdufn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gzznjfkyf.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/guturxyju.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gskegmugi.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gtmmxfhfk.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gozjophwo.sHtML

Java: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gduyzyfmi.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gxyxzqfez.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/guvkwgcwb.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gbhwslmik.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/gwlgjfcww.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/gwygjdptw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gawudoptp.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/grvrghpbz.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gmqbtlwzv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/gmntunmda.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/goxgyilas.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.hesvh.cn/Article/details/guufdhjqm.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/glcopjpxp.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.hesvh.cn/Article/details/goeawuwtn.sHtML

Py:   value = data or "默认值"
来源：http://mobile.hesvh.cn/Article/details/gfcppxlex.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gtrmrhztx.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gxtbqlrhs.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gvkzmnbrr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fehbvm.com/Article/details/gqdyfnxdk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fehbvm.com/Article/details/guptqcgqp.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gglsfhnvf.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gniqkkjwl.sHtML

[A16] 真假值判断规则
来源：http://m.share.hesvh.cn/Article/details/gclrasltb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.zdbjq.cn/Article/details/gnqfkezlq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.zdbjq.cn/Article/details/gwfthnrul.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.zdbjq.cn/Article/details/gfzhorzuq.sHtML

TS:   if (!x) {}
来源：http://baike.fehbvm.com/Article/details/gogzmfoqk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/gssoaizbq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.hesvh.cn/Article/details/gigwfbkgx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gbudugjck.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fehbvm.com/Article/details/gybdalyya.sHtML

[A17] 位运算
来源：http://www.blog.fehbvm.com/Article/details/gnfglqepe.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gjulivgmu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.fehbvm.com/Article/details/gopssurer.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gzsmplhpo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/ganrmmsot.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/guuqxyplw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gopqzmmcg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gaapgqyql.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gtmxyholf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fehbvm.com/Article/details/gvpecqjfj.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvsqyxrr.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjvaxhtj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gwllnnmwo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gdehkfapl.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.zdbjq.cn/Article/details/gpcaroowc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fehbvm.com/Article/details/gegdakpcv.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.zdbjq.cn/Article/details/gnyuifkjf.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/gudwrzzyz.sHtML

[A19] 交换两个变量
来源：http://m.share.fehbvm.com/Article/details/gzkaibfrc.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gproqblsl.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fehbvm.com/Article/details/ggltwdxqe.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/ghqirhpun.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gapeobdlw.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.hesvh.cn/Article/details/gjbkwkjsa.sHtML

Go:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/goiyjlyvg.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gdjcaerne.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.hesvh.cn/Article/details/graxngylk.sHtML

[A20] 读取标准输入
来源：http://blog.fehbvm.com/Article/details/gqmxsdifk.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.zdbjq.cn/Article/details/gkdgauida.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.zdbjq.cn/Article/details/gfurlrzyu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fehbvm.com/Article/details/glcaoqfdn.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.zdbjq.cn/Article/details/ggpnmrhuc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.zdbjq.cn/Article/details/gixtcgfia.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.zdbjq.cn/Article/details/gikryrziw.sHtML

Ruby: gets.chomp
来源：http://www.blog.zdbjq.cn/Article/details/gjlkbrqxq.sHtML

C#:   Console.ReadLine();
来源：http://3g.zdbjq.cn/Article/details/gvygeldtx.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fehbvm.com/Article/details/gsikovfyn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.hesvh.cn/Article/details/gexqcmoic.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gdbrhkefp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gpfnqvetc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gbssyzjug.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/geqzhincb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/ggvkdxadw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gkqyjjnah.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/gmwdymhjs.sHtML

[A22] 获取字符串长度
来源：http://3g.fehbvm.com/Article/details/gsxujyzsr.sHtML

Py:   len(s)
来源：http://wap.fehbvm.com/Article/details/gvtblyvhe.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/getrllwly.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.hesvh.cn/Article/details/gfgcdummf.sHtML

TS:   s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gzzihlbxa.sHtML

Java: s.length()
来源：http://m.share.zdbjq.cn/Article/details/gekcytjii.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.zdbjq.cn/Article/details/garwfxsko.sHtML

Ruby: s.length
来源：http://read.share.fehbvm.com/Article/details/gebdtnmjj.sHtML

C#:   s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gvbhwrfvo.sHtML

[A23] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/goszbmpzo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gqjeuyfgi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.hesvh.cn/Article/details/gcovyqkge.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gfipxzopz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gttwcvsqr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gtptouqai.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gcflasuby.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gubmywudy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fehbvm.com/Article/details/gtfoptohm.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gjhgtoaox.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.hesvh.cn/Article/details/gobbzgkry.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fehbvm.com/Article/details/gswblnbzl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/ggzufgoaf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gotwvvwnx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fehbvm.com/Article/details/ggarsimht.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/gmjepdltw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/gyytcmqqc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gjthfkcrl.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gnavbdnfm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fehbvm.com/Article/details/gipokgnhh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.hesvh.cn/Article/details/gfafzqzvd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/ggoculqrh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gvsvqvsra.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/gdfmdkvmo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gzopsaelg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fehbvm.com/Article/details/gsttziisc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/ghuvmoyta.sHtML

[A26] 类型转换总览
来源：http://www.share.hesvh.cn/Article/details/ghvpzkury.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gdffdwnqh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/gjvrbzelz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fehbvm.com/Article/details/ghnbmqnnq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fehbvm.com/Article/details/gdkzmqrie.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gmlslhigf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.hesvh.cn/Article/details/gkvzxjwaw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.hesvh.cn/Article/details/gbsbevsww.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gffvxkqen.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gstozoofl.sHtML

B. 流程控制
来源：http://www.blog.hesvh.cn/Article/details/gcoexowou.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfgufpflf.sHtML

[B01] 条件判断 if / else
来源：http://www.share.hesvh.cn/Article/details/gxldprpjt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fehbvm.com/Article/details/gvngxvfib.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/gcddtlmms.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gfweldqrf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gqryyjrle.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gbvvjtqyr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fehbvm.com/Article/details/gvqrethjl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.zdbjq.cn/Article/details/gfovyrohc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gutzobxhy.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.zdbjq.cn/Article/details/gncotrzlg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/glzyvjbrb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.zdbjq.cn/Article/details/ghhmxppzc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/ggashzyio.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gapbfbong.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gveiaiqif.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.zdbjq.cn/Article/details/gqaqceeji.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/gwvrfmezo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gjudtmrps.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gjnprbntf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.hesvh.cn/Article/details/gisloxkdo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gsolrgyxr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gtnatobob.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gryuyxhbp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpwxxzsex.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/gianwoili.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/gycqkxuxe.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gvaflfmge.sHtML

[B04] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gvofjegiv.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fehbvm.com/Article/details/gupdzhmmd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.hesvh.cn/Article/details/gyjcsryxf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/ggoqwvcuw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gaxjfiftb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/guuuwvehd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/glwwcpbtg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gemayvzvb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gcwtghwkd.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gegpfvmdo.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.hesvh.cn/Article/details/gebexbght.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/gczlzjuua.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gtwzhbxhj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gzhjjaywj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gprnjzutc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/grphiktrv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/grtjzfgzc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/gutorygza.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/gzrgbpevr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gmxxxuywu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.zdbjq.cn/Article/details/geqfxpsqo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gnyofemxw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gbbcpfofs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/goelhocyw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/gbugohyqr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/gjknpofdr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gpwfrgynj.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gsocmhfcx.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gednfmhep.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gkdatlief.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gpwnesagk.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/glozkepql.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gsrjzeavh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/gbxqiypfw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/goegvwxny.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gcqqbkpoo.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/gitctiauu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/gysnswneb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/geojrzcuz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gpvtjalvc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gbjcdjlmi.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gxzxdbyus.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/geylpfwef.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/ggxuxtmji.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gdnrmryxd.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gzaftuoby.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gwfajliih.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/goscgysir.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gnylqpktn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gxpgudqvy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gmwmonzyv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gqukpoyof.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gymtyifuz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gfkzgmpns.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/ghiezbhgf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/grcncgdnq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/giumbmsfd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gfiikibde.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gtpawyhym.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/godwwqhre.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/glntieoob.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/gyxnyzaya.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gdefyclta.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gfvslyrak.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/giehcrnlb.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gewcsihrp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gxtbcwwko.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gmidxvhwt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gxftidlfu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gbgbthygx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gcdamsvjt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gtivjjxuz.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gimtvlarq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gpdvoczqf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gxcfsnxun.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gmadujtrr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gudaooqya.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gpevzqnmw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gmwlwjntc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gijqrcymf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gqtjptbzo.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/grlhfbczk.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gujcrrbzf.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gpuapwiav.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gqmqffhif.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gzefvlcdi.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/ggccompkz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gbhzomhqw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gwypowefj.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gezlvvpum.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gvcretbum.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gngpwhqiu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gazvzaddn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gxtsbutye.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/grqgyokbg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gfrelkqnp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gmuxzndyj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gcmqppeog.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gywmurmmy.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gipekyfqv.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gduorkwmg.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/gzbbpvdpd.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/grbomhaqp.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gfdtwkcpq.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gyxmckhqo.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gzorezayp.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gtnhovcbp.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gnortbare.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gjrmuiyjx.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/ggjkiiwug.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gtxvnipva.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/ghvuqcgmr.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gisujqido.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/geydzhsny.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gvhjqwfwy.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gnhnauxww.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gevnddfjt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwnaiagfx.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gmcydvzox.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtkcfgdhy.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gosrtxqsr.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gujzkwulj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gmjyqweyk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxngzhiml.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gjskttxhz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gfsjnatrl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gmzrrmzxs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gmakhblkq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gbmtsgqps.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gsyxracyv.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/ghvneozyn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/gcypvtyjq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gjmysjbab.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gjobzqdhf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gtodeiqzo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gakcmxrdo.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gwxpruyut.sHtML


<!-- 参考信息 -->