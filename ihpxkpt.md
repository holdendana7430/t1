代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gjglbfvds.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fanxiaobao.xyz/Article/details/gpxnxdqin.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfcioczk.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fanxiaobao.xyz/Article/details/gqafueown.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyzvqfrm.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gfacqchsp.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzctxzbqz.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gjwahhyog.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgzrcmki.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvqrtbak.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcjczazn.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gzdgzperh.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyeovxzn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxxoaobn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gjarrkuvb.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvnkkprn.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gynyoukoo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkqqcndn.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwzniynz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxrlccuk.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgbtejws.sHtML

[A15] 空值判断与默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gifviqqxp.sHtML

Py:   value = data or "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/gpsbxsapb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/geeychwky.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gqfskajyq.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gayaknely.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fanxiaobao.xyz/Article/details/gebqpuycg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fanxiaobao.xyz/Article/details/gdudpvgzq.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gtmanuubq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagenvodx.sHtML

[A16] 真假值判断规则
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsqlzuye.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fanxiaobao.xyz/Article/details/gybllqgtq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbocckajf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fanxiaobao.xyz/Article/details/glnxccwzj.sHtML

TS:   if (!x) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghyzhvtfy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhiagird.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fanxiaobao.xyz/Article/details/grkfqulgu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gugapekdu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyhfblvcs.sHtML

[A17] 位运算
来源：http://wap.fanxiaobao.xyz/Article/details/grlwaifdn.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gccoujrfi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpficzis.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/giqmmcccw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgtqqbdy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/grmwjxcoi.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gagulzffm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvxdtfjx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmhwgjlj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fanxiaobao.xyz/Article/details/gjztjqicb.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzbajlwl.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gruceiitu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fanxiaobao.xyz/Article/details/glkpmfffw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gechdvywm.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fanxiaobao.xyz/Article/details/gmulykslz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fanxiaobao.xyz/Article/details/gymbepzkb.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fanxiaobao.xyz/Article/details/grqwexabk.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fanxiaobao.xyz/Article/details/gcpprsgeo.sHtML

[A19] 交换两个变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabwtqdeh.sHtML

Py:   a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gcwervzah.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkbvzykd.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmphdlmta.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fanxiaobao.xyz/Article/details/gskqpgjwy.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fanxiaobao.xyz/Article/details/gkrecrptr.sHtML

Go:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/guqpisupa.sHtML

Ruby: a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqukjbyy.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gllfrxapn.sHtML

[A20] 读取标准输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdphxdly.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnshevte.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbuwfsfw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fanxiaobao.xyz/Article/details/gnltqgdge.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/grvtcqskm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmcatqay.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuukeqmf.sHtML

Ruby: gets.chomp
来源：http://blog.fanxiaobao.xyz/Article/details/gzstrjwif.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fanxiaobao.xyz/Article/details/godbyrmfy.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fanxiaobao.xyz/Article/details/gkxljdjfu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fanxiaobao.xyz/Article/details/gutncimrm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmyeyfhp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtnvbzbb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gedqaoazq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fanxiaobao.xyz/Article/details/ggqnpslif.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gztrhznzz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gewhpgnjr.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fanxiaobao.xyz/Article/details/gaboezppu.sHtML

[A22] 获取字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/giahumzyy.sHtML

Py:   len(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpwkbabty.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fanxiaobao.xyz/Article/details/gdehbudpk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrmwuvpb.sHtML

TS:   s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gitplqqrs.sHtML

Java: s.length()
来源：http://3g.fanxiaobao.xyz/Article/details/geyqvxurb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gixvmxwgb.sHtML

Ruby: s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgxhychw.sHtML

C#:   s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpqnhyae.sHtML

[A23] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvyqkqnq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fanxiaobao.xyz/Article/details/genohqahc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqjzepll.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gciocmspt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdzelrpp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjielwzi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmnnaziq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/goqxffvjk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fanxiaobao.xyz/Article/details/gsflxhqvh.sHtML

[A24] 去除首尾空白
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqatbafp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fanxiaobao.xyz/Article/details/gxzqbjtic.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfhookbi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcykvnymr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrsucemj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjdthlrf.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfelhmpxj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fanxiaobao.xyz/Article/details/gvuzmiigm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsiailgq.sHtML

[A25] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gccgwnpvf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fanxiaobao.xyz/Article/details/gsysdrvbm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gzzyfnndz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggduvsvpg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyagmlggs.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gupwkpeph.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzolqcwbx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fanxiaobao.xyz/Article/details/gdtmwjwrp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzizqrwjh.sHtML

[A26] 类型转换总览
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpgghkvx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfiydskk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fanxiaobao.xyz/Article/details/gixecsigg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fanxiaobao.xyz/Article/details/gwwfsxful.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fanxiaobao.xyz/Article/details/glzeptgyl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fanxiaobao.xyz/Article/details/golclrpqj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkqikciw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gvnyixdjl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/geoaatidn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtchwmey.sHtML

B. 流程控制
来源：http://baike.fanxiaobao.xyz/Article/details/gqbotftgd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjicbdadi.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsodflsc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqwcwkjp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcoakerir.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbmeibic.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzoyxdkl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gctrzeguh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyflemqsz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gydkvzovv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gunwuqdwk.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjlnjgdp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fanxiaobao.xyz/Article/details/gimwxrcwu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpujjxlp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gloufldjb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfztialy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gbvrgwccs.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gopmlajhl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/geigrswey.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlcowimk.sHtML

[B03] switch / match / case
来源：http://wap.fanxiaobao.xyz/Article/details/gmwrftwln.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgsuxwrs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcsefegtj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsfryrlm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggdfjgrob.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvuynurk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gsarncuui.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtuxnxzz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgqjdzsx.sHtML

[B04] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwpgjvbl.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuthwmdm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gleubxlhn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gowvdfdfe.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbjujkop.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxhpkemm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvemnsquk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkghkuyud.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiymfbqj.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gqahhvmlb.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fanxiaobao.xyz/Article/details/gtonjpigf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gonqipkmq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/grphyricm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnovgrbcr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/glmyndzoo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gembcrhzs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fanxiaobao.xyz/Article/details/ggbeoqpxy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gerulfbvm.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gldvfuvpg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gikusxzpr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfthpgrch.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gztiafrrt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfcaxbyw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/goaulwvhu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasfftvma.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fanxiaobao.xyz/Article/details/ghzzelgqw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmkksxom.sHtML

[B07] while 循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gndlgadvx.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggicykudr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvjqeoid.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggwedbzkv.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gruveihih.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqugkrzp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgbytkvo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fanxiaobao.xyz/Article/details/gpjaackwa.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gklxtsskk.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmqsruip.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fanxiaobao.xyz/Article/details/gdnxpfkie.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihdfvwto.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gsutpjjdi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gkcmexwbb.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gdotphdlq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gydammwhg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fanxiaobao.xyz/Article/details/guzooialp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwwfswpt.sHtML

[B09] break 与 continue
来源：http://wap.fanxiaobao.xyz/Article/details/gwqjekdzf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyesxxjd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftjkermh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gapcijiar.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzokdqxl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/grrrshaki.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgpuayah.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fanxiaobao.xyz/Article/details/gmfcajulj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvihcnia.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxmycbio.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gieezfmoc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyztkxrzh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasqyikxh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gbcodnggw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fanxiaobao.xyz/Article/details/guztipnyr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fanxiaobao.xyz/Article/details/gxrnfecwl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmdfahfq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkgjioiz.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fanxiaobao.xyz/Article/details/goeyfhaad.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gekiqsyqq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjggeqmw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gorargftj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjftdajic.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmtnncgx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctvzqwxb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/girgzmcma.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaajfdntp.sHtML

[B12] 跳出多层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdoccjgo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqyainwd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fanxiaobao.xyz/Article/details/ggqvabsne.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gyfumcvjq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gvfulltab.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvduocbdk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmymnxktv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjpjodgt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqptijsf.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gplrfrkmu.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuxtrpoi.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpvlvoxf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gtybepvgd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gekwsertj.sHtML

Java: x instanceof Number
来源：http://baike.fanxiaobao.xyz/Article/details/gsknvfqey.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/gypozcpwj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbxiqzbr.sHtML

C#:   x is int or double or decimal
来源：http://3g.fanxiaobao.xyz/Article/details/ggigozjef.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyrnhvll.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvbhalse.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fanxiaobao.xyz/Article/details/gohzkzkqi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/glbiqwrmw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gzdwipxzg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gntbvgjhk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gspemeqsq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmltwxwrk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/glqqzuvlp.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhmywqpc.sHtML

Py:   a and b or not c
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnwafhgz.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdrohguh.sHtML

JS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgwrbvlj.sHtML

TS:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gymicpmvz.sHtML

Java: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybvxoukx.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzngjsur.sHtML

Ruby: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/ghbdlmcqb.sHtML

C#:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gmluwgwgg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfezejvu.sHtML

Py:   if not data: return
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyakuaqc.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmccupbmi.sHtML

JS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gvhbkjuxk.sHtML

TS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gwjvtesoh.sHtML

Java: if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpejnerv.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxotsqnu.sHtML

Ruby: return if data.nil?
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqwgoeby.sHtML

C#:   if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gocqvfhsd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvmfstomd.sHtML

C. 函数与作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvkadpuh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwjuulsy.sHtML

[C01] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhcxqzqn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gzltxbwby.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmodfxmcb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxothosg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpgmkcpbn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmrrejwr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gelgabdgw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnodtqhbb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggnoowwkp.sHtML

[C02] 默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtassujcd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gisprhonx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gigujtpno.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkxwiprpl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gluxnieyl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdwzflid.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggssswhuy.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpfzcsgk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fanxiaobao.xyz/Article/details/gzprjfsyd.sHtML

[C03] 可变参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfzzrjvs.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fanxiaobao.xyz/Article/details/ghgkhlcim.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fanxiaobao.xyz/Article/details/gpgtkwnyc.sHtML


<!-- 参考信息 -->