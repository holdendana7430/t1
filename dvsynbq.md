代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcvgyfax.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gzdlalpys.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrbvwxho.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbfuutxxg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fanxiaobao.xyz/Article/details/gvrhayzwn.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fanxiaobao.xyz/Article/details/gkbxcljxz.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwasspnl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fanxiaobao.xyz/Article/details/gxrmsaxsh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmhlsrby.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkezliedv.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fanxiaobao.xyz/Article/details/gcnvqijcf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcapxdgh.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkclktlsc.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaimbbon.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gznatcnfv.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gytpbkzzg.sHtML

Java: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gfmpvlyvo.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gdpcvxogs.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmugaspur.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gttbhuzct.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgrkjeqv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllxcbkym.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gpchzzobx.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/grvlxbgpo.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqygectt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fanxiaobao.xyz/Article/details/ggrrgnnog.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/ghzfipfgi.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fanxiaobao.xyz/Article/details/gktxwgglz.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gkwckviza.sHtML

[A15] 空值判断与默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gttofilvc.sHtML

Py:   value = data or "默认值"
来源：http://3g.fanxiaobao.xyz/Article/details/gqstlnjeq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gctbwbkyz.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuygpzvp.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gxfgfybcf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fanxiaobao.xyz/Article/details/gwkywxubp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtrmdqny.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkdovjqq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyczwmns.sHtML

[A16] 真假值判断规则
来源：http://wap.fanxiaobao.xyz/Article/details/gwuipnhmv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fanxiaobao.xyz/Article/details/guvcoxxvo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygkbvbvo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fanxiaobao.xyz/Article/details/grcsvenaq.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guciqelxv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfnongqq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvpzuxng.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gyldxirkd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfuqjwrv.sHtML

[A17] 位运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwwnauva.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfalbayku.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/guqiaxekv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpbaryxw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnukrhdka.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpzuumhm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifpfcihf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gbvfqnqpg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkghzemo.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhxrvapa.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmygrrpfi.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpozqhfek.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbsrafdm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/gehhwysww.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqntwevl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fanxiaobao.xyz/Article/details/gsipksjtf.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fanxiaobao.xyz/Article/details/gaqisuvrh.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fanxiaobao.xyz/Article/details/goggfeasz.sHtML

[A19] 交换两个变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqedzdmfx.sHtML

Py:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiedpnqo.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fanxiaobao.xyz/Article/details/gazjzqztm.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkpbxala.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fanxiaobao.xyz/Article/details/ggninapbx.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fanxiaobao.xyz/Article/details/gjzvifkhg.sHtML

Go:   a, b = b, a
来源：http://wap.fanxiaobao.xyz/Article/details/glvpichzb.sHtML

Ruby: a, b = b, a
来源：http://3g.fanxiaobao.xyz/Article/details/gdyzvelzq.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fanxiaobao.xyz/Article/details/glvunltqi.sHtML

[A20] 读取标准输入
来源：http://baike.fanxiaobao.xyz/Article/details/gkocgltio.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffzthrhz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fanxiaobao.xyz/Article/details/gomtvhjgt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqhmihhy.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gkxcrmcfi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbbbcdta.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fanxiaobao.xyz/Article/details/gyqkmcgso.sHtML

Ruby: gets.chomp
来源：http://m.share.fanxiaobao.xyz/Article/details/gclushglx.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fanxiaobao.xyz/Article/details/guednfilh.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fanxiaobao.xyz/Article/details/gscixfevp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvvikjyt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fanxiaobao.xyz/Article/details/gqwukveph.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfkfgipq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/ggutvvbew.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gdfsxcoel.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwndpdipc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsisswupv.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fanxiaobao.xyz/Article/details/gdktpeyot.sHtML

[A22] 获取字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnqsmltp.sHtML

Py:   len(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gplarwdjb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fanxiaobao.xyz/Article/details/gyrpuewqf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fanxiaobao.xyz/Article/details/ghykxtmtx.sHtML

TS:   s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gblezduzn.sHtML

Java: s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtodwurvx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpuivqmc.sHtML

Ruby: s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifierwjq.sHtML

C#:   s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoxlbddl.sHtML

[A23] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gvwlohytb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gpjestkkl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwglqfma.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbklvtrsm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgxypcbw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.fanxiaobao.xyz/Article/details/gevikbqno.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfmsfzsb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fanxiaobao.xyz/Article/details/gydepnhta.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthceycwg.sHtML

[A24] 去除首尾空白
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxlzxdrt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxodbxyj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvfohinu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/glkgqaexg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/golwwlmls.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fanxiaobao.xyz/Article/details/gyttqvwqv.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gopyfgurj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbotdgglt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfslepcbf.sHtML

[A25] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gcizqyleo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdteircnd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsuqaoce.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxhwfdsk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gbewtfank.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxgqzbpj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcejecobd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fanxiaobao.xyz/Article/details/glfozzlvr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvirafsa.sHtML

[A26] 类型转换总览
来源：http://mobile.fanxiaobao.xyz/Article/details/gnibtweqg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fanxiaobao.xyz/Article/details/gttyakhrw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhhigzdz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fanxiaobao.xyz/Article/details/gjghjvytm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fanxiaobao.xyz/Article/details/gxxwmbqku.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gfzzizwih.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fanxiaobao.xyz/Article/details/girvxkxrh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gkbnqcket.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpheywpds.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeuzkizk.sHtML

B. 流程控制
来源：http://read.share.fanxiaobao.xyz/Article/details/gsflmpxti.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gikooimbf.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrxrmqga.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyikyebd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwdjxphv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gpebfuwvw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/goqjsbrsk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/grmhltpgf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtihfcvzk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrhebjpb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/glkmsaxko.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcwcqilq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjigsdnr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsxsxpdo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqaaujti.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gznwqsaoj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayfinvrh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxvokkfe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fanxiaobao.xyz/Article/details/gjffbsdkq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnqpwuuk.sHtML

[B03] switch / match / case
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjuoukpa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fanxiaobao.xyz/Article/details/gshzarelc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsqykwhkw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gurzmbykg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyrvqqgf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkskyvjlf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgixqfiz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpnfvwuw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gutjqdeft.sHtML

[B04] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/goitprjqv.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwtjqskk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjnmnpisu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gkpgkpecq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gpoeewkvg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gajvbnyjc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fanxiaobao.xyz/Article/details/gwhobcxsx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoaduxui.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gxxbxtbhp.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxvlruzq.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fanxiaobao.xyz/Article/details/gstbqqwrp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gousscgkf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjldprjtw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gdbfpiwfq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gnyzhitrz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjfegjqp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fanxiaobao.xyz/Article/details/gscgwfada.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfubzgyrk.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fanxiaobao.xyz/Article/details/getbewwsh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldfdgcvs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grhgbxwog.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/geenqbvjm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gquejgkdp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gbmwjtnqz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpzprysb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gswszuwrh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gztcqcwet.sHtML

[B07] while 循环
来源：http://mobile.fanxiaobao.xyz/Article/details/genybhqqd.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/guaknkotl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmygcubzc.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvjhskcdh.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvswjliu.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzflvcduk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpxgtihu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fanxiaobao.xyz/Article/details/givupspjs.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtipmjuj.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fanxiaobao.xyz/Article/details/gaukjzbpc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fanxiaobao.xyz/Article/details/genzzipkf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjnzefrj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/glkbqzbls.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoukougt.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gkyibohqm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/ghwcdxzjk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fanxiaobao.xyz/Article/details/gqtsccolr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdihkiqf.sHtML

[B09] break 与 continue
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzbmiqkk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/gydupjmxt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmuxrgmn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkztanqte.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpyvhofzc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghbsoomui.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gvhhxwzew.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrkhswmg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/guheqvjbm.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fanxiaobao.xyz/Article/details/guwiabrjo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqkbzcqb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpakaspwp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/glcgbwucp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gndtyymto.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fanxiaobao.xyz/Article/details/gjnsubqgi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fanxiaobao.xyz/Article/details/gvyivnral.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqhuhqen.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbsjwcqik.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fanxiaobao.xyz/Article/details/gorjlsynv.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnqyuaze.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gurqocrza.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegekwajz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpyvlbnw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfesnzgg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxtzqjft.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchrhpval.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gehkdhqwl.sHtML

[B12] 跳出多层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/grjgginkz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/gutzraisr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/govvdevht.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gafbjwvjz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzwujmok.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxwhkfck.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmnzqwhn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gyddhpkpj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fanxiaobao.xyz/Article/details/gbxdhhzmm.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipkeebie.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fanxiaobao.xyz/Article/details/gphyuntxp.sHtML

PHP:  is_numeric($x)
来源：http://3g.fanxiaobao.xyz/Article/details/gidfychqc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gpkocabnd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gfsoareaj.sHtML

Java: x instanceof Number
来源：http://wap.fanxiaobao.xyz/Article/details/gogagghdb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkskrynho.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekjztgav.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/gakobfxdp.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fanxiaobao.xyz/Article/details/gizvylrmi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfwrbtxw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fanxiaobao.xyz/Article/details/gabkiqwlw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gptmkepih.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gobidxehw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijaqdieb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqvqliyo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gzvknhhtv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gslwyaqul.sHtML

[B15] 布尔运算与取反
来源：http://wap.fanxiaobao.xyz/Article/details/gvirrzaxw.sHtML

Py:   a and b or not c
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtbuddcu.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbecidxi.sHtML

JS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gewnilrik.sHtML

TS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliyyjgge.sHtML

Java: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gagjjkyyj.sHtML

Go:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkypgxtpv.sHtML

Ruby: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gncnwtvpt.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gaiiulizb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gprrgdhjv.sHtML

Py:   if not data: return
来源：http://m.share.fanxiaobao.xyz/Article/details/gwquisvgh.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhnxcnjf.sHtML

JS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/ggvehutpw.sHtML

TS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqzopepy.sHtML

Java: if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gadfdgfwg.sHtML

Go:   if data == nil { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgciicdq.sHtML

Ruby: return if data.nil?
来源：http://3g.fanxiaobao.xyz/Article/details/gyiertiuo.sHtML

C#:   if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gzxkymfrb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfxzkjnnw.sHtML

C. 函数与作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gipgebymx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvacaaedm.sHtML

[C01] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwiisqjjw.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gxiinfllh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gedzpmvzd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/grphpfupo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbfgfyna.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcslluqe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvazcmget.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fanxiaobao.xyz/Article/details/gpwbthwrh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkfyfzewz.sHtML

[C02] 默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpefiqbn.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fanxiaobao.xyz/Article/details/gmfvwjuip.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkrchmlf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghigywqhb.sHtML


<!-- 参考信息 -->