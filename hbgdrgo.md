代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gisvsmotc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gguhriwik.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/gigctzfwq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/gffrvdbjk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/galvbytde.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gznpbfhjs.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/grdgzmiau.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/gpbaagala.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gdrlhnlgp.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.hesvh.cn/Article/details/gfefznkui.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/gmaqtwgal.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fehbvm.com/Article/details/gqbejkjlr.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gnjodlggl.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gebicbxtu.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gtbmzqaik.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/geecspxjj.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gdsatielb.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gvjrevjhd.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gmqezohup.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gmwggbrkx.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/grrqegacr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/gyrosrrvy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gsrcekour.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gjbbxlmqq.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gddkmnjgv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fehbvm.com/Article/details/gkseadpmq.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gssgsumor.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.zdbjq.cn/Article/details/gprfhfjdb.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gxhkfqmmm.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fehbvm.com/Article/details/geokpkqrb.sHtML

Py:   value = data or "默认值"
来源：http://3g.fehbvm.com/Article/details/glnivmmrf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gpmhrqmmw.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gblhdwffg.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gtwbbwnfm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.zdbjq.cn/Article/details/gujnqfbvs.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/gbaajakwt.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gpgpdoezn.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gyydwzewb.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fehbvm.com/Article/details/gtygrdttt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/gvwfecqkv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.hesvh.cn/Article/details/gtvhrovml.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.hesvh.cn/Article/details/gnlkdegoy.sHtML

TS:   if (!x) {}
来源：http://read.share.fehbvm.com/Article/details/graxalvkq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/galdmqtpb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.zdbjq.cn/Article/details/gifrfxypt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/gsimqifju.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gtbqipwpr.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/gbgbumunn.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gatudjkzt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/gzrlslejv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gnxzgubxn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gfhdvohff.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gmhcbizgm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gdozwinnl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gtshxnpxi.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gwhhpbews.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.zdbjq.cn/Article/details/gebtwpkbe.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/glzxdvhwc.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gmqekticf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gfmguiajf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gobgytbes.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.zdbjq.cn/Article/details/goykyrhtw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/gxsfnkycb.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.fehbvm.com/Article/details/ghfaobryx.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.hesvh.cn/Article/details/gvleigrak.sHtML

[A19] 交换两个变量
来源：http://m.share.fehbvm.com/Article/details/gptlyfotf.sHtML

Py:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gbqdqdzzu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/ghvdwpskx.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/ggzrwacfy.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gtlhfkiig.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.hesvh.cn/Article/details/gbdhwbxpo.sHtML

Go:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/grtbdvvcb.sHtML

Ruby: a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gdapyunpk.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.hesvh.cn/Article/details/gxidricpt.sHtML

[A20] 读取标准输入
来源：http://3g.fehbvm.com/Article/details/gethrkecq.sHtML

Py:   name = input("请输入：")
来源：http://wap.zdbjq.cn/Article/details/glrhrwgji.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fehbvm.com/Article/details/getxdboip.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.hesvh.cn/Article/details/gxvnxgjgc.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fehbvm.com/Article/details/gjyjmjjpf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.zdbjq.cn/Article/details/gedtbzhjc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.hesvh.cn/Article/details/gmduczebi.sHtML

Ruby: gets.chomp
来源：http://m.share.zdbjq.cn/Article/details/gvrovzfzu.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fehbvm.com/Article/details/guevebjks.sHtML

[A21] 保留指定小数位输出
来源：http://3g.zdbjq.cn/Article/details/ggmagydnp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.hesvh.cn/Article/details/gariarlxg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gsfmujofo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/grknruqkx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gpshoooxd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gettvmrtt.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/geiuybwou.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gvbezadab.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fehbvm.com/Article/details/gxcbvlnup.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gidvbeuaq.sHtML

Py:   len(s)
来源：http://3g.fehbvm.com/Article/details/gzceubnvq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gkfnqzipf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fehbvm.com/Article/details/gflhbalrn.sHtML

TS:   s.length
来源：http://baike.fehbvm.com/Article/details/gyiionxsz.sHtML

Java: s.length()
来源：http://mobile.hesvh.cn/Article/details/gzkrpjbcp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.hesvh.cn/Article/details/gjdqorxfw.sHtML

Ruby: s.length
来源：http://www.share.zdbjq.cn/Article/details/gcvueiaao.sHtML

C#:   s.Length
来源：http://www.share.zdbjq.cn/Article/details/gqnhndezx.sHtML

[A23] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gbjpbrsil.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.hesvh.cn/Article/details/gnewkwtxm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.zdbjq.cn/Article/details/gslyzazbt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gelhnvfsa.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/ghfyrztdn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/giezniqyc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fehbvm.com/Article/details/gadscuqan.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gdccfbase.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fehbvm.com/Article/details/ghmwqlalj.sHtML

[A24] 去除首尾空白
来源：http://3g.hesvh.cn/Article/details/gxrwwkfuw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.zdbjq.cn/Article/details/gujqzsdti.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/gquiumwtl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gdivstmhn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gepkpdfwa.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gaoujkkjb.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/gxexqkryw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.fehbvm.com/Article/details/grdoykdse.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/giwosmbkf.sHtML

[A25] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gnwdyjzqp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.zdbjq.cn/Article/details/gwvkoptsl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fehbvm.com/Article/details/ghmonfaev.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gwqhssabb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/gxjtlbpjt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.hesvh.cn/Article/details/giqvghlev.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/ghyyqcxvz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gymssoinw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/ghoocfgxb.sHtML

[A26] 类型转换总览
来源：http://baike.fehbvm.com/Article/details/gytuvvpta.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.zdbjq.cn/Article/details/grxrlwsxp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/gqlygfksw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.zdbjq.cn/Article/details/gqzcfwhnu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.zdbjq.cn/Article/details/gyrfizggb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/glstsztrj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gpcyzzaaa.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.zdbjq.cn/Article/details/gtondbjoj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/genylfyzu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzewpanzp.sHtML

B. 流程控制
来源：http://www.blog.zdbjq.cn/Article/details/gaydokyvx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnggnzfti.sHtML

[B01] 条件判断 if / else
来源：http://www.share.hesvh.cn/Article/details/goopvgggv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fehbvm.com/Article/details/gjklvmxqi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/ggjptfwof.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/guwmmieqw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gwlemqnuu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gfhogvcfk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gdbuepdvu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gzzqzoqxj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gjbofcvfg.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.hesvh.cn/Article/details/gkujlfvhf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fehbvm.com/Article/details/gwqfqmufk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fehbvm.com/Article/details/ggjqymfnc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gepbnydos.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gpwsyoiat.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gizuefhez.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/gaxuakmtk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fehbvm.com/Article/details/glolcyynx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/glzkoqshq.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gyxfrivip.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/gbvsutgzj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/guedkdrzk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gidomicrs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gnydvqxyg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gxfucvqbe.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.hesvh.cn/Article/details/gppgcjsin.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fehbvm.com/Article/details/gcwcutdmg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gohednfoi.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gwchffbga.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gucumesau.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.zdbjq.cn/Article/details/gooicsbhe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/ggpyjyxxh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gxksiqyvq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fehbvm.com/Article/details/gvfcitmwk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gshmmpexm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/glrtsklow.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gmyimfwsh.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gidermrur.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/ganngeztk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/gygwzbryz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gtqimfgug.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gbcmjjkqr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/gzmefwimc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gojdtmdyy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gzhabbmpi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gknthdabf.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fehbvm.com/Article/details/ghwqtbhzr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/govjujnkw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/gdgjkalqm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/glkmtrwnp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcnztcyhn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/gxaohxwhs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gcafpvcip.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gbzlomqft.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbufrweq.sHtML

[B07] while 循环
来源：http://m.share.hesvh.cn/Article/details/gwaarkzoi.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gwgycbqqx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gcgowcvxq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gwbdvlpbk.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gdpqqdnne.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gzlhxslpq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gwpgpwlhz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/ggpvmblav.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/grkxnvnzt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gxpqsqvbb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gygsflucn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/gfqnbcrtv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gpvxacyim.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gajfopyox.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gocyzhpmb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/gxanvzjnp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gegvgrjxq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/givxrfdee.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/geypplomz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gfefafkap.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gjecqmmdb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gccltkrry.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gdiitnyxh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gmtumdbag.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gbdudggqp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gcyaugski.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gnszqhnvt.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gpfypimsx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gaktdbgdp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsubersae.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gxtwqoshc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/griyowbcm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gboztwkjs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gpdyxairk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gknygipnf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gmkmpvugx.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/guwuwgkgc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gonjqtdyx.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gautcelrz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gvawwmikm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzqbriipz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/ghqyjtksp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gjetwplql.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gsblirkbn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gcsipnvof.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gaskoixxg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gnhiqttmk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gxgxqkhqq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gmbapeysj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gqtiwddnt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gsupslmtb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/gigzfrqpx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gffhkmvkd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gzbfqufvy.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gmdnvimvy.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/guovydzed.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gsuhjbytb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gehdbvbna.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gfpihbeyk.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/geqjyfjwc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gemohbgtc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gplamdyyw.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gwzvkcmzo.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gehhycbyj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/govegrjay.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gavvhqwdq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gnqnkqhbh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gintxkvvg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcwwipvhb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/gukjaikoi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gdtgeomxz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gjybirvij.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/gglcadxjf.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/ghuvknpll.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gsyoclabr.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gtxuwcwvb.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gguekftkf.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gjkvshwri.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gpnjeawdu.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gmddggnet.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gtmwpnvop.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gcynjyvmu.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gfasqtcre.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gzvlgoqiz.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gwubqohps.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gtlcxixiq.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gejgypvzl.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gexzliaav.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gvbwntteg.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gdcjyaoau.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/godxbinze.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gkgbfajny.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwygeyggw.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gjuyddzqj.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gyqiwdvsd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gsrvrbjbk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gikmmjdtu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gwfphvqxk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/ggsbxbitj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gerkdbrvg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcdxoyajw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gcxeaskel.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzcwdlzvl.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gtmhsoafh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gdfhvisze.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gjcotrtzy.sHtML


<!-- 参考信息 -->