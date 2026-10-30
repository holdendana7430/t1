代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gtilihkwn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/geoebyhub.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/ggzqwnqio.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gglevujmw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gpklfkmsy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/glsppiznh.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/gqgjrrvpn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/giqkoizfv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fehbvm.com/Article/details/greuhfhcj.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gpodhanep.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gghldreqm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.zdbjq.cn/Article/details/gyynclfyn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.zdbjq.cn/Article/details/guopresnj.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gyfgxrjjb.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/gqyljybcr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/gzxlgngna.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gbvtryihl.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/ggpazknmq.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gzagicpfg.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gflifjabu.sHtML

Java: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gpdbfxzgt.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gtxawnsyi.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/goyvekcxp.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gttvoxgqk.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/ggrnrmpql.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.zdbjq.cn/Article/details/gjuwwyief.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gbyxtojxu.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gszicrdrb.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gbraqtbkg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.hesvh.cn/Article/details/gdwosvsel.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/glmhinyuh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gbjliefdp.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gseaxlinz.sHtML

[A15] 空值判断与默认值
来源：http://read.share.zdbjq.cn/Article/details/gafzfezqd.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fehbvm.com/Article/details/gnedunyqg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gryjkewve.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/geivezxyn.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gpobnqvrs.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/goqhilhgp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fehbvm.com/Article/details/gvgqrjrnf.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/gmskflzcg.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gpybewwon.sHtML

[A16] 真假值判断规则
来源：http://wap.fehbvm.com/Article/details/glscqxchs.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gqyslxtur.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gqwjfdevl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.zdbjq.cn/Article/details/gqaspgygn.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gvhsoioxd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fehbvm.com/Article/details/grhapnqle.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.hesvh.cn/Article/details/gkpyitypb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fehbvm.com/Article/details/gmeunvmiu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.hesvh.cn/Article/details/geqiuircu.sHtML

[A17] 位运算
来源：http://3g.fehbvm.com/Article/details/gaebgkgjr.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gudoeqwsp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gtgphdtoy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/glczebxxb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gleykqruj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gziauestn.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gmpovemgl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gedvartfn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gqflxkfaq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fehbvm.com/Article/details/gsynijths.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gwgjxwike.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/ghsnnqtwc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gtjzserif.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/grikhtmnr.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.hesvh.cn/Article/details/gnusfxdiz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.zdbjq.cn/Article/details/gfbmwcmbk.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.zdbjq.cn/Article/details/gytmpfpjb.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.fehbvm.com/Article/details/gvnxarutz.sHtML

[A19] 交换两个变量
来源：http://baike.fehbvm.com/Article/details/glznjkxpq.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gobjzwcxu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.hesvh.cn/Article/details/ghqavfsbo.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.hesvh.cn/Article/details/ggcbjkakn.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gbhanfddi.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fehbvm.com/Article/details/glbkhgiwb.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gsnrykhpm.sHtML

Ruby: a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/gfdeaoftb.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.hesvh.cn/Article/details/gcqrradhz.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fehbvm.com/Article/details/girporjbg.sHtML

Py:   name = input("请输入：")
来源：http://blog.zdbjq.cn/Article/details/ggvdrajtj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fehbvm.com/Article/details/gzhrhgndb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fehbvm.com/Article/details/gctcgvxmr.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.zdbjq.cn/Article/details/gfhwcklud.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.zdbjq.cn/Article/details/glswxckod.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/ggboxnmql.sHtML

Ruby: gets.chomp
来源：http://www.blog.hesvh.cn/Article/details/gsbkjvsqi.sHtML

C#:   Console.ReadLine();
来源：http://wap.fehbvm.com/Article/details/gsvdkiybb.sHtML

[A21] 保留指定小数位输出
来源：http://blog.zdbjq.cn/Article/details/glyahhita.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.hesvh.cn/Article/details/gpbfigvmt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gahbtgjxe.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gqnmmzefo.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gwuycmruw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gtfvkhsxg.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gghexvvuy.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gvhczypjk.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fehbvm.com/Article/details/ggmnhhhuk.sHtML

[A22] 获取字符串长度
来源：http://www.share.fehbvm.com/Article/details/gulqhtjjl.sHtML

Py:   len(s)
来源：http://www.blog.hesvh.cn/Article/details/gtmwcidjy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/grhmtjptl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.zdbjq.cn/Article/details/gkephyftk.sHtML

TS:   s.length
来源：http://wap.zdbjq.cn/Article/details/ginjjnlia.sHtML

Java: s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gyhazovgd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fehbvm.com/Article/details/godmlnlew.sHtML

Ruby: s.length
来源：http://3g.zdbjq.cn/Article/details/gprkjvzcm.sHtML

C#:   s.Length
来源：http://read.share.hesvh.cn/Article/details/grwndqtix.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gpepvjtpg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.hesvh.cn/Article/details/gzsrckmke.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fehbvm.com/Article/details/gwuchrfnu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gdlcitmnk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gsiccixlw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gzmfwozic.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.zdbjq.cn/Article/details/grssmcips.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gmcbforza.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.zdbjq.cn/Article/details/gnqesffqn.sHtML

[A24] 去除首尾空白
来源：http://blog.hesvh.cn/Article/details/gsevuxtmg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.zdbjq.cn/Article/details/gfposlqiq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkicawvok.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gmmfxzpdg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gvwwfytii.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.hesvh.cn/Article/details/gotjcgfle.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fehbvm.com/Article/details/gnxftgmzk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.zdbjq.cn/Article/details/gfebiqkxi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.zdbjq.cn/Article/details/geluvurgj.sHtML

[A25] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gkxmhzbuk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.zdbjq.cn/Article/details/gaunrtoub.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fehbvm.com/Article/details/gtmtktzdr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gxibxclkq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gfdlkmdux.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/grgruqlcs.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gtczsflrj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.hesvh.cn/Article/details/gbgxcrjra.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gngkjyqat.sHtML

[A26] 类型转换总览
来源：http://wap.hesvh.cn/Article/details/grufeeeel.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/gnrtqezto.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.zdbjq.cn/Article/details/ggtgqdlza.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.hesvh.cn/Article/details/gshlspyhu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fehbvm.com/Article/details/gkqvrydcw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gjwsfyuac.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fehbvm.com/Article/details/gzxrfanej.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.hesvh.cn/Article/details/gyrioqull.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gxhtlfapr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grkpoidfx.sHtML

B. 流程控制
来源：http://blog.hesvh.cn/Article/details/grblzekqs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gktvprgfq.sHtML

[B01] 条件判断 if / else
来源：http://mobile.hesvh.cn/Article/details/gjuzqmogk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.hesvh.cn/Article/details/gawzkmupc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyrszvrky.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gehrwftrd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gejeqwuhq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/glyioldyo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.hesvh.cn/Article/details/gcbhaxdlf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.hesvh.cn/Article/details/gkkujxhyo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gzmnkcdea.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/gselmvkpv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fehbvm.com/Article/details/gjywlcmom.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gtxmjgbkz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/goxcshfxi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gxxpchogs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gdgwboppp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.hesvh.cn/Article/details/gxpjgkzxv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/gvgrwxavv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/ghznsxcej.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/gwedtsffy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gtredhhkx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gmvfaaetp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gibhmvhkq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/goylmhyuk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gftiniozq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/govkoesdo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.hesvh.cn/Article/details/gpnjqkolu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/guxyptthc.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gnlvvxmbw.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/ghnowgwmz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gggdqgugs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/ghjjsvguy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/ggvakrbmi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbvdpnmi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.hesvh.cn/Article/details/grqlvxkwe.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.zdbjq.cn/Article/details/gpfhxvlqt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/gcdhvctbk.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gntbuxpqv.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gonqggfuf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.zdbjq.cn/Article/details/gvvcxvnqo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/grhkfmtkz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gjruuwjlt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.zdbjq.cn/Article/details/geunagddw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/gaqhyrmjj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/glcjvypvv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fehbvm.com/Article/details/gyfdiwegl.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.hesvh.cn/Article/details/gttiqirdr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/gomczpraq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gwkwbpcpj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gkstujdmk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gaxxbgdon.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/guknnwitu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gbgkxsvoq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gfindpyqc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gpnzxhuol.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gwuooiitt.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/gonqnvvxg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gghzenygc.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gsqaitvdb.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gdbasfapv.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/goanzimfm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gcibifsfp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/gnhpbklzx.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gqrsjgcfb.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gwqmcyoro.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gzidmwtsh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/gvypgtadv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gjnbhvsym.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/girrjfmuz.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gcbuzajhc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/gpwcjliby.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gvujntema.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/graabqadd.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gklqvhlgo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gsjwkczta.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gsesjenqu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gdtzzcjun.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gugdusgsa.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gkkcibodg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gcilsadjh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gbyqbzgux.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gekkesejx.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gngylehfc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gbekvqion.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gytuegrlv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gcbiqkpzc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gpohtwkqt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gptakwlhd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gwotcrxxz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gxooxypkl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gfzphzysg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gaemvbgow.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gsvvkkbhh.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gdoddkuae.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gkbwgjeju.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gjxlqmfht.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gwjacqvyu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gtlotngrv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/grnusqxcs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gefhxxoii.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gkupogdkt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/grmvmlzoi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/gpnfyxlud.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/glyzaohir.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gllzhwsrd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gbpcswnpv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gesavyayy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gbgtntdnq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/gtwmikqvg.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/glwjfucde.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gmxoovqxf.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/ghujdgqxr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/glpfahdkn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gremkdtxu.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gingarfwp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/ghtmuysoc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gkjjhglbz.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gcrogzbwd.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gecxnimww.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gwegtkfhg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gpxxcpeuc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gcezjvwzq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gespyfeza.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gsbvliyyo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gtlzimial.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtxugpptf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbcowrgct.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gewexdhbs.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gcwbqgrav.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gqtjmgsaq.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/geotjvbmy.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gvcsnrgna.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gujyprpur.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gthnropgm.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gozqrzzmb.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gqjubektk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gnpizwqzd.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/glovublbq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gutnxryla.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gmvpoitnq.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gnedntqml.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gcrtfrrnf.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gcepahzld.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/guturlbuh.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/glejcdbzn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gspuodfsg.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gpcrgeosk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsgjqlymt.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gmypcwhlo.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gxuixgnsx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gnrlxotml.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/grtyoptye.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gukpozmtl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghzbeixwu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gmlaxwxku.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gsqizovzy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gfotjrdpk.sHtML


<!-- 参考信息 -->