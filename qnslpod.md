代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gvhuccqhj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gxlpwvvkj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gjpukudrw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/gpdwpndvd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/ggqkmvhqz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gwouyjhbe.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.zdbjq.cn/Article/details/gmpppaczl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.hesvh.cn/Article/details/gxlnzylvd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/gagzgdsto.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/ggfiipvop.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gobxgmuht.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/gskwrshoe.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gjyhqygjf.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.hesvh.cn/Article/details/gjuucezob.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gduyutkzg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.hesvh.cn/Article/details/gexlfktkg.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gdhhkpoig.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gmnjrufer.sHtML

JS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gupzgvdtx.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gcjibktih.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gcevwpnco.sHtML

Go:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gjdxjojln.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gfpybznzw.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gizknzcpr.sHtML

[A14] 注释写法
来源：http://wap.fehbvm.com/Article/details/gwvqbzpyg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/gteminqwe.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/glpryyatu.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gzzlmrbra.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gdjpnskhq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fehbvm.com/Article/details/gmlxmsimx.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/ggfnagbha.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fehbvm.com/Article/details/gyuvchkks.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gxsnkmlhc.sHtML

[A15] 空值判断与默认值
来源：http://read.share.hesvh.cn/Article/details/gqmbbthmj.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gudrzqyra.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gyxjmexin.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gzcdxarrl.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gpvyxlcqc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fehbvm.com/Article/details/gywwltwce.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/gagprggcn.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/gfbzjoixi.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gsuvkjvxn.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.hesvh.cn/Article/details/gvckjbzvb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.hesvh.cn/Article/details/guxiapfwg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.zdbjq.cn/Article/details/gnensuycc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/gyxgicqen.sHtML

TS:   if (!x) {}
来源：http://www.blog.fehbvm.com/Article/details/gichxnswv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fehbvm.com/Article/details/gqeskopqz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.hesvh.cn/Article/details/gnwohmzvl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fehbvm.com/Article/details/gcoypxzjz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/glffwgnje.sHtML

[A17] 位运算
来源：http://www.share.hesvh.cn/Article/details/geylzkgvw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gjdrgvpvq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.zdbjq.cn/Article/details/gqlfsezdf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gkbgyvcwu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gbrxjrujx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/guhcijcsc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gvitlxzse.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/ghdxbmnsb.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/geyepdrva.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/gkzvsjskc.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.zdbjq.cn/Article/details/gntxlzbfs.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gbvefeilj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gbxjcgswk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/ghcgngxmj.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.hesvh.cn/Article/details/ggxvfzrcp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fehbvm.com/Article/details/gssxchjhd.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fehbvm.com/Article/details/gbcorvfan.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.zdbjq.cn/Article/details/gjrayvddw.sHtML

[A19] 交换两个变量
来源：http://read.share.zdbjq.cn/Article/details/gajxtvxnt.sHtML

Py:   a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/gmbeyumjt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.hesvh.cn/Article/details/gwotiaozs.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/girmowifs.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/guvzguslv.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fehbvm.com/Article/details/gvaaefcyj.sHtML

Go:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gmjjdykwu.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gblagxkjb.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fehbvm.com/Article/details/gkadmyphp.sHtML

[A20] 读取标准输入
来源：http://www.blog.hesvh.cn/Article/details/gnpbzdies.sHtML

Py:   name = input("请输入：")
来源：http://blog.zdbjq.cn/Article/details/gzsgnvhud.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.zdbjq.cn/Article/details/gruzgtdyk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fehbvm.com/Article/details/gvohhxltt.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.zdbjq.cn/Article/details/gefwmzyya.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/gsloxfayu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.zdbjq.cn/Article/details/gwzlnrljw.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gucnxetig.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gqdeizhrc.sHtML

[A21] 保留指定小数位输出
来源：http://3g.zdbjq.cn/Article/details/gvaalfpez.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/gahbrkyli.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/grjifvkoe.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/ghplicder.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gcnofrdwu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gulqvziyl.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gtnjiessv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/geuxntjmk.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/gjejnhajl.sHtML

[A22] 获取字符串长度
来源：http://blog.hesvh.cn/Article/details/gvnwveyhg.sHtML

Py:   len(s)
来源：http://www.share.hesvh.cn/Article/details/govutyckm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/ggjeilbvx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.zdbjq.cn/Article/details/gqwpyaobb.sHtML

TS:   s.length
来源：http://wap.fehbvm.com/Article/details/gqxwoknaw.sHtML

Java: s.length()
来源：http://read.share.fehbvm.com/Article/details/gzlcuhhzm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsxoxlkhk.sHtML

Ruby: s.length
来源：http://www.blog.zdbjq.cn/Article/details/gedxtshfa.sHtML

C#:   s.Length
来源：http://read.share.hesvh.cn/Article/details/gfydcdnvi.sHtML

[A23] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gydfbetwf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gijldhfce.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fehbvm.com/Article/details/grabtpvnb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gttnfsncf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gitjggovs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/ggbdtdemf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gcfqqrnxt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.hesvh.cn/Article/details/giaxzzblt.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fehbvm.com/Article/details/gixflmnbj.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/giojvtpkt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.hesvh.cn/Article/details/gssqqpaxq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/gpcakbvmo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gvkzfldlc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gsiptsxvq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.zdbjq.cn/Article/details/gbtvltbgl.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.zdbjq.cn/Article/details/gwsmdpslz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.zdbjq.cn/Article/details/gvdymwlki.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gbphxwxqo.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gczluppyr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fehbvm.com/Article/details/gsajfgcpg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzrrfabb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gromyrtle.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gggquktau.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fehbvm.com/Article/details/gjlgiuaqt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gudartrlg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.hesvh.cn/Article/details/gdhlfrtjj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gqdtkyupx.sHtML

[A26] 类型转换总览
来源：http://www.blog.zdbjq.cn/Article/details/gtgygxphb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.zdbjq.cn/Article/details/gpoobfooc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gqcyesjbe.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/gaabmyxif.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.zdbjq.cn/Article/details/gqvifslng.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gtampvhde.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.zdbjq.cn/Article/details/gegixrlql.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.hesvh.cn/Article/details/gjzomyejr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gzeslxzom.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gignovtnj.sHtML

B. 流程控制
来源：http://m.share.hesvh.cn/Article/details/grcslabiz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glilcujvl.sHtML

[B01] 条件判断 if / else
来源：http://www.share.hesvh.cn/Article/details/ghgnzjxho.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/glutxubzf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.zdbjq.cn/Article/details/gmazslzsh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gkxibhxvn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gftigkcfk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gxjcqedqu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.zdbjq.cn/Article/details/gvgyedvno.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.hesvh.cn/Article/details/gneudpiqm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gjwdvhvbp.sHtML

[B02] 多分支 else if / elif
来源：http://blog.zdbjq.cn/Article/details/ghjyjdrgb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/ggkwjziyy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/gixnehijv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gmruphamm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gydubwwzy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/ggvrowcwj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/glrpvcatt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.hesvh.cn/Article/details/gbnvygynx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gxeupkcfn.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/gtrkhidug.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.zdbjq.cn/Article/details/gsfbfkjyb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/goijllbyt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gqhotpdby.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gaxfajkmi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gxxmbgues.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/gyazmndnk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fehbvm.com/Article/details/gqxgngsfc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gxmmuwmed.sHtML

[B04] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gfyalmohd.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.hesvh.cn/Article/details/gliiserry.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.hesvh.cn/Article/details/gyoejmocm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/guimpawpe.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gdnguqctz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.hesvh.cn/Article/details/gqhtemlee.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gtezyznve.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gikgccxnk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gjphyupfw.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gqqvbrait.sHtML

Py:   for item in arr: print(item)
来源：http://3g.hesvh.cn/Article/details/gshgdrxbo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcrzclbsk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gctzmvurd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gqwyqohrb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gjdohsbbz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/gjgkwrucf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gbinmpysh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/gxcapsbtd.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gtosysopg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gzoiihwej.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmbmhgehe.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gsmfqcajs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gbxkjcawy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gjdfetigd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/gpbtclxge.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/ggrizrrue.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gvhhaivvl.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gnfgdpopr.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gyoumheut.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/gheeeqzry.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gswnmxrsv.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gskiatxpe.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gfzzzxypy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gdnfknkfg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gultzkyys.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gcifnhoes.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gxsctvuzr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/ggmmuxuni.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gktqtecky.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gizuugmyy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gypxozmzm.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/grblhbvwk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gxlllzkfh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gbwjtpnrm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gjmqccypc.sHtML

[B09] break 与 continue
来源：http://www.share.hesvh.cn/Article/details/gszsephnd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/gwebjiikg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gaqrgxnuf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gmefeqbxx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gjyjkiwfp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gbqxksxhv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gzphuxgix.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gpgzcpngc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gzohkfsay.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gikgjsixg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gqkhglrvq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gaodsauaa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gsmmxdcpa.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gfwjsianm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gifgobkkd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gulfgultc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gosnsfhbs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gjoszzmdq.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gvieqtbju.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gyhsbgzyg.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gfctceped.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/ghpeeeueq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gqtjkgzyb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/ggcyierly.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gutuyefhd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gbivzsnzf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gasoshhxf.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gtrwdhvfz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gcwyjmghl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gpuecxkaq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/goivcttvo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gvmuyabui.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gojydcrex.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gglctvtjy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/grkhuksxb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gadilgluj.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gynjkgteq.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gubjmletg.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gxwjyoxxm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gxsyuyjfs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gcogdsflb.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gnbtruvep.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gphnappky.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gtusnxywr.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gzzzacbjd.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gnpilgqmv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gjumrolqd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gpbnpcizw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gnehmwkyu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gcqzmsqsx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gxpbsscqy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gbahlxjjg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gurtqiism.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gddifgbmc.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gyjusqzzz.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gbqrjkjar.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gixwwjidn.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gwzjhsgbr.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gnbepoqaq.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/giaftbadt.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gkttyhsln.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/glxoxktzl.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gdahrxisq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gdtdnjppx.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gnanxjhgm.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gpdetdzdm.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/guwbcgmtl.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/grmjyoalj.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gsdtwovpj.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gcbmtrsha.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gcsojemyh.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gmwticejp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggxytoeat.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gurkhftaj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gavgkejpv.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gpmotjxkg.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gsdxapkzc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gxajrmbbe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gmmokxqkw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gamlqiovs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gmvuszjwg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gaxwxywwo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gsysmqqca.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gjzlazusb.sHtML


<!-- 参考信息 -->