代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gzmghyqpl.sHtML

[A11] 条件表达式（三元）
来源：http://blog.hesvh.cn/Article/details/guzavojvg.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/gnaijfqhf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gffuozoik.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gjogtznwf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gvfoyrzhq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gmsltdyej.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/gjjmtikhf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gsxdfjowp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gfousjhzt.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fehbvm.com/Article/details/glrlnjqyh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.hesvh.cn/Article/details/gmeiluevx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/gwzpgwzvs.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gochuqgck.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gbffainmi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/ghfyixvzt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.zdbjq.cn/Article/details/gvlxtpezl.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gqktdhdyt.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fehbvm.com/Article/details/goacoapqv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gxazwtpbx.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/glykogyep.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gksrmcvqr.sHtML

JS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gojbfietq.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gealozxvb.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gvsyahvok.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gyawjozon.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gaipyiehv.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/grtmrekmm.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/gouobbidm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.zdbjq.cn/Article/details/gvoktbuij.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gelhgdsov.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gvpmybehb.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/ghvpfjhmz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gehfbemgt.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gergikegz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fehbvm.com/Article/details/gnebihfqi.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gujdmjarm.sHtML

[A15] 空值判断与默认值
来源：http://www.share.hesvh.cn/Article/details/gqbducqfi.sHtML

Py:   value = data or "默认值"
来源：http://m.share.hesvh.cn/Article/details/gamsqvkqg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gwzkwjila.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/grrwpprlt.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gwtbshtez.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.hesvh.cn/Article/details/gofqaigqd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.hesvh.cn/Article/details/gbipepavh.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/gabgvdmus.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gsjshlahg.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/gvlrfgunw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fehbvm.com/Article/details/ggrggysey.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/gxvqhdylt.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.hesvh.cn/Article/details/gajhdlfug.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gtjelgxop.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/gibzmzjze.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.hesvh.cn/Article/details/gytenobip.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gjotvbrze.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fehbvm.com/Article/details/gmgbxocqc.sHtML

[A17] 位运算
来源：http://www.share.zdbjq.cn/Article/details/gpggyzpuz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gukmnywxg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fehbvm.com/Article/details/gdvcxwfed.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gkhjwbtpx.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gfdkdzynw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gdmaqdkel.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/goqtgmgtm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gaxaansnv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gmdpqkyyb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.zdbjq.cn/Article/details/ghqyzvlsh.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gaipcikrc.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gtiomrica.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/geddvscxn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/gjiahsdwn.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fehbvm.com/Article/details/gbhjlsmdk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.zdbjq.cn/Article/details/gpqnwpqro.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.zdbjq.cn/Article/details/gqqylkieh.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.hesvh.cn/Article/details/gagxejfld.sHtML

[A19] 交换两个变量
来源：http://www.blog.zdbjq.cn/Article/details/ghvsmetip.sHtML

Py:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gsvedynen.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.zdbjq.cn/Article/details/gfadnmyac.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gekljujfd.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/ghnfzqowi.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.hesvh.cn/Article/details/gqwoyshtj.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gckfbvtew.sHtML

Ruby: a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gwnukxefl.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.hesvh.cn/Article/details/gbdexswzu.sHtML

[A20] 读取标准输入
来源：http://baike.zdbjq.cn/Article/details/gecggegjt.sHtML

Py:   name = input("请输入：")
来源：http://baike.hesvh.cn/Article/details/gfhpinlrc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fehbvm.com/Article/details/gvyujmyks.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.zdbjq.cn/Article/details/gbzwrhfes.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.hesvh.cn/Article/details/gnhwhtetz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fehbvm.com/Article/details/goiextfpe.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fehbvm.com/Article/details/gzobthybt.sHtML

Ruby: gets.chomp
来源：http://mobile.hesvh.cn/Article/details/gvojuuqgj.sHtML

C#:   Console.ReadLine();
来源：http://wap.zdbjq.cn/Article/details/gyyyxqjqb.sHtML

[A21] 保留指定小数位输出
来源：http://wap.zdbjq.cn/Article/details/guswajtvp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.hesvh.cn/Article/details/gskotcozd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gwngmpzwe.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gzgkhjucw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gryjgriai.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/glamjekrz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gvznjkvsc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/ggvoafsiq.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/gfginhzhx.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gdaxpdiel.sHtML

Py:   len(s)
来源：http://read.share.hesvh.cn/Article/details/gkbzslixr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.zdbjq.cn/Article/details/gfqmsrvbo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gzgdeswbr.sHtML

TS:   s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggmfeiyde.sHtML

Java: s.length()
来源：http://3g.zdbjq.cn/Article/details/gdscuapwn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.zdbjq.cn/Article/details/gmwsoznef.sHtML

Ruby: s.length
来源：http://mobile.hesvh.cn/Article/details/gqxwokcur.sHtML

C#:   s.Length
来源：http://baike.hesvh.cn/Article/details/gjgwcoyhe.sHtML

[A23] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gccbnkfgv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fehbvm.com/Article/details/gxdmxhyrq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.hesvh.cn/Article/details/guqbdvjet.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gjuwxpjbe.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gklqskdss.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gyahilqnb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkdltakwe.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gsjmszntf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.zdbjq.cn/Article/details/gldviorvx.sHtML

[A24] 去除首尾空白
来源：http://blog.hesvh.cn/Article/details/geswcwcgt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.zdbjq.cn/Article/details/gzigpzpie.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxrqapyh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/ghnozzmed.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gpsjmzywt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.hesvh.cn/Article/details/gsmwizrtp.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnwpsupaw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fehbvm.com/Article/details/gioltagrw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fehbvm.com/Article/details/gbzsuqzpl.sHtML

[A25] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gvexhkvim.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.hesvh.cn/Article/details/gqizodkni.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.hesvh.cn/Article/details/gzdbpldqg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gagoabtss.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gbsyufwnu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.zdbjq.cn/Article/details/goowcghah.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gtilumeya.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.zdbjq.cn/Article/details/geznsvstq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/glbauqmnn.sHtML

[A26] 类型转换总览
来源：http://baike.zdbjq.cn/Article/details/gtnxvrveo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/gslqlvbui.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fehbvm.com/Article/details/gyyocoiqk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fehbvm.com/Article/details/glpdogxtj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fehbvm.com/Article/details/gxiekynhh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/glyvscinv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.hesvh.cn/Article/details/geckpgaws.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.hesvh.cn/Article/details/ggxlzjbnk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.hesvh.cn/Article/details/gnglwqgbf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwtavjdkp.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/gnlpsmptk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcqgdvmqu.sHtML

[B01] 条件判断 if / else
来源：http://baike.zdbjq.cn/Article/details/goyrnjhic.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/gfxwafmzq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.zdbjq.cn/Article/details/gbczyldzd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gmfcmgjor.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gfribonbh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gazlmohpf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fehbvm.com/Article/details/gmwukarre.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.zdbjq.cn/Article/details/ghsisjwfs.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gvclxikkc.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gpnlecefy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/gadramwpd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gymwjifax.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/glrsqvohr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gryidlumb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gonhuhwle.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/gesuuwdiu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.hesvh.cn/Article/details/gqqhdacjy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/ggwiuwbto.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/ghylyjhzf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gabjnfbbs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gqurfcicn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gqrsjhddu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkokugwev.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gmxsyrahf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gjilofoyg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.hesvh.cn/Article/details/gntnqoxfu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/ghbpmlkeg.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gbbajdnus.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gajrruvqn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.zdbjq.cn/Article/details/glsynailp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gsanaviio.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/grtatphjc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gmktcjdzx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gbdsybuhh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fehbvm.com/Article/details/gnjgccpns.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.hesvh.cn/Article/details/grwufnnal.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gfrsfkufz.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gsvbvfdxz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxqpfrlrh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gkcyjgibo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/glsfbkmbk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/gkzamoajp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.hesvh.cn/Article/details/gcbhzronu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.hesvh.cn/Article/details/giuaxpjia.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gjdzehawo.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/grmucsqpy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.hesvh.cn/Article/details/gcefvybrw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfbzbcwvg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/glcwbqpwj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gyoolmahq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gbcooxtif.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gylgsdvev.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gcaimzwzr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fehbvm.com/Article/details/gmqeqkhvi.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/gecdthhqq.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gophlevtt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gtarlxxzh.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gujxzelze.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gkysggmmt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gnuhpjxat.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gskfgcqvm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gvdykpklh.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gmggiizfy.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/gyuwhzerd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gbgafaupa.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/grubgnprt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gifajctkv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gcrjaiaqs.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gyiimhbmi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gnetdlmpz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/grzsmmrsg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gvqbdyphl.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gsufdinmq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gibfmyvog.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gfgmwkjhc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/grtcxdxxd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gmuvfzlcr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/grdtqslul.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gpfzlagqe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/ggwupiffd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/ghxascsri.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gllyyteme.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/gynrqbcrc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghwvnlbtw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gbigfomic.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gbkfpicac.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gwhqqstru.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/grcdofmum.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/gztuovfix.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gqoapmqkz.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gmdrypstp.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.zdbjq.cn/Article/details/gffrbhhsz.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gyqkgaqew.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/ghfbbvakj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/guwezhpod.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gnwbwobhj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gdwuirono.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gpllepfau.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/ggydhggjb.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gnslppjpt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gecjnbmhe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gsnqicwhb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gyacxpkpp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gxppzdllz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gvameocbd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/giupdcvyk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/ggyaqglqi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gznhcdlhd.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gjdwolirv.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/ghsmfqwqa.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gbrcrvxan.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gssiaytcx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gparvcwft.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gyozrjfga.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gweotsfpc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gckkwmzeb.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/ggzcnarqn.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/ghstxdgla.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gwxdhesqb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gttcccbif.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gmhdkvswa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gfwaopddr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gpxexesmd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/ghycpktlx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/gsispiqrs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/guijdtbct.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/geatdpakm.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gacccsuqp.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gmyrwgzsp.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gfhadxqpr.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gewppkfbf.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gzftlvwqj.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ghoyphgxq.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gvesxqnsd.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gdyvjxcdn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gdvvxqjcl.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gjwmcuepy.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gwexnlyig.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/ganiwxpia.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gwrguwjwk.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gimbejcho.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/ggfcudnhi.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gjdvvttwo.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gapfomhgz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnacmgyke.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gzdjcoeda.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghcepclca.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/ghpcvzgxy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gcbuponez.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/geusrkwqf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gpqfsqqhr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gggtlshqz.sHtML


<!-- 参考信息 -->