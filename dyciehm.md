代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gjxjsfajl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gdvpzbhzj.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/geodhjkhf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.hesvh.cn/Article/details/gnsvcargy.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/gnpinznui.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gjqkfytos.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gpzzohxuj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.hesvh.cn/Article/details/gxvtfhurp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.zdbjq.cn/Article/details/gtjstjodv.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fehbvm.com/Article/details/gwabwwkwx.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/ghriyhdps.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fehbvm.com/Article/details/gxksstyop.sHtML

Py:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/glhiymnmr.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gnvbdhynh.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gjwwhvxyh.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gabvfcxav.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gdgqbaslf.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gjyldsheb.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gmgiahwil.sHtML

C#:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gzyqoswkm.sHtML

[A14] 注释写法
来源：http://read.share.hesvh.cn/Article/details/gfjqsjmhx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/goasanovu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/giohkckpm.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/ghictjlgv.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/glvbylryk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/gxqtvxuuk.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gjtoiqvug.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.zdbjq.cn/Article/details/gmmmdsjqj.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gyiwrsgns.sHtML

[A15] 空值判断与默认值
来源：http://read.share.zdbjq.cn/Article/details/gngvcrywh.sHtML

Py:   value = data or "默认值"
来源：http://blog.zdbjq.cn/Article/details/gyxmpmyzu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gzwdmnklu.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gjtkfxrfy.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gqvzrifzv.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.zdbjq.cn/Article/details/gbrjhmcuv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/gulaaycwy.sHtML

Ruby: value = data || "默认值"
来源：http://blog.zdbjq.cn/Article/details/gqjhnfxtq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gisoljzer.sHtML

[A16] 真假值判断规则
来源：http://3g.zdbjq.cn/Article/details/gnfyzptwj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.hesvh.cn/Article/details/gnyfkejow.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.zdbjq.cn/Article/details/guqnftxok.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/glrsmjvnq.sHtML

TS:   if (!x) {}
来源：http://baike.hesvh.cn/Article/details/gnpwsigiu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fehbvm.com/Article/details/glolmumgs.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/ghtfiyrgm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/gzzapipux.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.hesvh.cn/Article/details/gceduzewt.sHtML

[A17] 位运算
来源：http://baike.hesvh.cn/Article/details/gtxqomfku.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gvavblxeo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fehbvm.com/Article/details/gunokkxmd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gxuzgrmvz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gsyffggsb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gvdujwctz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gppwiyogy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gqjrhpyom.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/girzdbjxa.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.zdbjq.cn/Article/details/gyvawxdok.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/glugflocm.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gdhpqxohi.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.zdbjq.cn/Article/details/gqlnapway.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/giakelnlq.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/geacguiso.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/gybhiaiji.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.hesvh.cn/Article/details/gssckygqz.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.hesvh.cn/Article/details/geaxzqiyz.sHtML

[A19] 交换两个变量
来源：http://www.m.share.fehbvm.com/Article/details/gdhdfjyje.sHtML

Py:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gjrqoybsy.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.zdbjq.cn/Article/details/gdqntayok.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/gkqkjucwn.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gchbkwmsg.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.hesvh.cn/Article/details/gcasggcdn.sHtML

Go:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gcaidqhal.sHtML

Ruby: a, b = b, a
来源：http://3g.fehbvm.com/Article/details/goeujlrsf.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fehbvm.com/Article/details/grdtpzqpm.sHtML

[A20] 读取标准输入
来源：http://www.share.hesvh.cn/Article/details/gjiocprmp.sHtML

Py:   name = input("请输入：")
来源：http://3g.hesvh.cn/Article/details/gbiarwtju.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fehbvm.com/Article/details/gkafpyrwp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fehbvm.com/Article/details/gbldufneu.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.zdbjq.cn/Article/details/gbncyaitb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fehbvm.com/Article/details/gfdgfwcxv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/ghqrajgxb.sHtML

Ruby: gets.chomp
来源：http://mobile.hesvh.cn/Article/details/gwpryoivy.sHtML

C#:   Console.ReadLine();
来源：http://blog.hesvh.cn/Article/details/gwsamxvzb.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.hesvh.cn/Article/details/gtcpqicun.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.zdbjq.cn/Article/details/gcmvmwkhq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gnlxkxxxt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gejlyvvdf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/ghslsibwr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gqgcwapht.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gegvqdkjf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gqcmbbiyj.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.zdbjq.cn/Article/details/gdiamxmym.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gorfuqhzn.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gwndxeunr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fehbvm.com/Article/details/gdvjuygnr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fehbvm.com/Article/details/gcpcsfhlk.sHtML

TS:   s.length
来源：http://baike.zdbjq.cn/Article/details/gvflnvdwt.sHtML

Java: s.length()
来源：http://mobile.fehbvm.com/Article/details/gvpkvwguf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fehbvm.com/Article/details/gyfycriom.sHtML

Ruby: s.length
来源：http://wap.fehbvm.com/Article/details/gpdrncqxl.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/gpbrlkdhi.sHtML

[A23] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gisseluzn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.zdbjq.cn/Article/details/gdsmsrpum.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/godfjxveh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gmefwfahi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gwgeepenj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gvdhlgckb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fehbvm.com/Article/details/gxmpgykhq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/gbxddihhh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fehbvm.com/Article/details/grwebdaps.sHtML

[A24] 去除首尾空白
来源：http://blog.fehbvm.com/Article/details/gojxnimnr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/gppgumaly.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.hesvh.cn/Article/details/gxeicrukp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gauczoayv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/grjckbaue.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.zdbjq.cn/Article/details/gpufqkdbr.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.zdbjq.cn/Article/details/gxlqaiyxd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.zdbjq.cn/Article/details/gjpdmjsom.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/gtgacsesa.sHtML

[A25] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gykbxmijh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.hesvh.cn/Article/details/gprdsojuz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/glsljsnjg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gottukxon.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gidkrtcif.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.zdbjq.cn/Article/details/gefwoqxqf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gmxmkdzoz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/grbngbgfb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/ggtrnhenh.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gjuslbyba.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/gzjyhrrqx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/ghgqeyeqo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gitjigfrx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fehbvm.com/Article/details/gqwwhqwer.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/ggxgpqkkk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fehbvm.com/Article/details/gffuomepl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gcfbamhbb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gzufilfjw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdattguhb.sHtML

B. 流程控制
来源：http://read.share.fehbvm.com/Article/details/grfjeaasa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqsjpicmg.sHtML

[B01] 条件判断 if / else
来源：http://www.share.zdbjq.cn/Article/details/gkpqlrlek.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gwgidkwtu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.hesvh.cn/Article/details/gamxmgbzc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gztdwugju.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gppvxdomg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/ghumrbixk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.zdbjq.cn/Article/details/gembdvvpi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.zdbjq.cn/Article/details/gflyxmswb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gxdhdlcff.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gejkgzxhv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.hesvh.cn/Article/details/grvxktcne.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.zdbjq.cn/Article/details/gelkqferm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/ghhmirrou.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gpctggncp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/ggpodjmgx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fehbvm.com/Article/details/gevecpknm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gamoihobt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gortmplsh.sHtML

[B03] switch / match / case
来源：http://www.blog.zdbjq.cn/Article/details/glxxykivm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/gsinazlsg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gltlmywpa.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gfjcfdpoy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gyzityvva.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gtntyokis.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gqlvtlkzv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/glrgoierb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fehbvm.com/Article/details/gjlupcbje.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gyryooxay.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.hesvh.cn/Article/details/gkaynayrz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/gdbtbljng.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/grsvpubqb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gmbwxkloz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.zdbjq.cn/Article/details/gsvtndkyg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.hesvh.cn/Article/details/gcjgauvag.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/guvbqqoku.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fehbvm.com/Article/details/gujsgrlma.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gnjcrbsih.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/gqhonucsl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggaqcaubi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkoychbnr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gafyftkib.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gruvwbdwa.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/gzxiiwbke.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/gvaakypcm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gkyvilehq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gprmgryll.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/gfzsgfijh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.hesvh.cn/Article/details/gdjhzgjnx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gzwwnuapq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gqjdowtzf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/ghqoueoke.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gsamilclt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gscojkjxz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gbhajfsqn.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/gjsznfonp.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gjvazqflh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gyygjajkl.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/glcjycmiu.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/glwlqfylr.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gbuywalzr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gglcelivi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.zdbjq.cn/Article/details/gasfaxeye.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/ghyuldhvo.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gcamfggax.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/gfmmrgoox.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.zdbjq.cn/Article/details/gxlgwendv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gnmnefrgf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gvjksmyah.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gukvuvkhj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gpuythdqo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gybrkminx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gfcemktou.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/ggzfokjfw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gnsehabtk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gvjajabyt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gakaeopav.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gedwbzdmv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gglxxdfrq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/ghjbnrucd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gzcvonbjq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gqhqaxedl.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gwntscmoa.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gxsxegpbt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/ggegfyviy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gohtlbsan.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gfhoqilcg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gqmivptap.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gasleyuyq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gdjpmnyht.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gkzseyugh.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gjzlbrrtu.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/gsihehvrr.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/ggybccexx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gjbjawndz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gqcvvxtho.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gvvndwrmx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/ghxshbehg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gmexcwnvk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gzvvqjgbc.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gddrqxnax.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/ghwhzfknx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gldnodzdl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gojjuxsfo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gihlcbidl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gyvlozpuo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gygjvthqp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gbqtwaasc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gvgozdcnr.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gdlkebses.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gipkstlsp.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gywippwtk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gqeqewbua.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gcjljejaq.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gxmrzixjo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gtkucvgxx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gpfjrabed.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gkrcryexh.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gkwtrsine.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/ggwnrhwle.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gxeboffwo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/grvjodczy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/grjjjimai.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gemghdhgo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gejxzekab.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gbporuugp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfxolnpxt.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gfhdgzxxm.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gwofuyzfp.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gdlbypgra.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/ggabyzyav.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gnzohnydi.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gewezidov.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gcqiscbqf.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/glemqbpvm.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gebzzplyf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gcylwujkh.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gfjzmpkgw.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gdcqfihsy.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gofpregfp.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gllnrarxp.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gputpoino.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gceklabfn.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gdnadxtlo.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gwmktgqxf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghafdtmpu.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gulaiteax.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfksuejxb.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/guddxfqls.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gtruzngug.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gjqegdcfv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gxjxuosir.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gwbaqozpw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ghbfpiffd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gdzcjgkyn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gbksulbdv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ghrrameth.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/ggsadonnb.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/giduroxgr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/glefmmkhs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gxyzeiqmu.sHtML


<!-- 参考信息 -->