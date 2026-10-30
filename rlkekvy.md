代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.fanxiaobao.xyz/Article/details/gdolvmkhi.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fanxiaobao.xyz/Article/details/gwbjjvhwp.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fanxiaobao.xyz/Article/details/gnmmdvmdi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gduihsaeq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gunmfcqek.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gadtrslnk.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fanxiaobao.xyz/Article/details/gkcfecmrp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnczuqnrn.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggihinpey.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gtkjqskpn.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gbieqwtfb.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlgtjyoc.sHtML

Java: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gmwtfoyww.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gisnrlizx.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gjcgkhpxq.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbcwyqae.sHtML

[A14] 注释写法
来源：http://3g.fanxiaobao.xyz/Article/details/gopqnynzd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fanxiaobao.xyz/Article/details/gwawmgiam.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gffpswqsa.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gurflwjhs.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwwpebfr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fanxiaobao.xyz/Article/details/gdjmyedod.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/geztxvrgc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghddbvilm.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gypeqfplh.sHtML

[A15] 空值判断与默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gmltbgamu.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvexooerw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/grvxeigyx.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzynwotp.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/guhvcwmth.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxxeergc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fanxiaobao.xyz/Article/details/glbdnykzq.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/gphpvyugb.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcpdkiln.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/gwicrklcr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gdekkicor.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fanxiaobao.xyz/Article/details/gedwtktrd.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fanxiaobao.xyz/Article/details/gbwrwftbs.sHtML

TS:   if (!x) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gprvmpazy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcncxfkd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fanxiaobao.xyz/Article/details/gzerlxiim.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fanxiaobao.xyz/Article/details/gigddadtf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfnthkazz.sHtML

[A17] 位运算
来源：http://3g.fanxiaobao.xyz/Article/details/greuzbtfe.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gvwfjrotz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/geqioxhqt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gbamwuzwj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmeezohm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/glhjnksjy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/giquthxxw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gugkfrnvd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/glrsfugjg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.fanxiaobao.xyz/Article/details/ghmenebvp.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fanxiaobao.xyz/Article/details/giibzlhun.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/greebgzsa.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gppusutce.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyphhytkn.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fanxiaobao.xyz/Article/details/gvawraixm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fanxiaobao.xyz/Article/details/gmubsovfa.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fanxiaobao.xyz/Article/details/gtspkizql.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fanxiaobao.xyz/Article/details/gqupvubvh.sHtML

[A19] 交换两个变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyakvwkim.sHtML

Py:   a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gaalwfqij.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaktaryr.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fanxiaobao.xyz/Article/details/ghgkemkou.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoujfhlz.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fanxiaobao.xyz/Article/details/gmcnnzkgp.sHtML

Go:   a, b = b, a
来源：http://m.share.fanxiaobao.xyz/Article/details/gbftbdozr.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrfgfara.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.fanxiaobao.xyz/Article/details/ggqbslviq.sHtML

[A20] 读取标准输入
来源：http://wap.fanxiaobao.xyz/Article/details/glolfeccg.sHtML

Py:   name = input("请输入：")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdthgmigm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fanxiaobao.xyz/Article/details/gavhurebf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fanxiaobao.xyz/Article/details/gkknphvbj.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gcspjknxl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqsswszg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkckcfomg.sHtML

Ruby: gets.chomp
来源：http://3g.fanxiaobao.xyz/Article/details/gtttyrwwj.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgczrcvg.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoingmbi.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcivbuasw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/ghdgzahel.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcskrderw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gnjumpfbi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmvushwu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdvikhfl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/ggvqrkcuk.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwkreqjh.sHtML

[A22] 获取字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrqkxrzb.sHtML

Py:   len(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghftiubkr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fanxiaobao.xyz/Article/details/gprnxdzta.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fanxiaobao.xyz/Article/details/giwilggpn.sHtML

TS:   s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaffogga.sHtML

Java: s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmrugumj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gduzqbliv.sHtML

Ruby: s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gjuvqgltt.sHtML

C#:   s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuzndecr.sHtML

[A23] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gpmfqvtue.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fanxiaobao.xyz/Article/details/gapupjakk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fanxiaobao.xyz/Article/details/gfpeoaooi.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gefdjbyxy.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrwozzdd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgzeyzth.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvltmrvuz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpxpkive.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fanxiaobao.xyz/Article/details/gpbnsfowj.sHtML

[A24] 去除首尾空白
来源：http://read.share.fanxiaobao.xyz/Article/details/gevgwzriy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fanxiaobao.xyz/Article/details/gicrfcmxr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmkbgeow.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gmzykdrvh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnfghtnd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fanxiaobao.xyz/Article/details/gloxeygym.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gltcocvmq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fanxiaobao.xyz/Article/details/gkktiedmw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gkpygloah.sHtML

[A25] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/ghojjqxae.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fanxiaobao.xyz/Article/details/gxlzvhagu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqcuyizfi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyndsfqb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fanxiaobao.xyz/Article/details/glapxvyle.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmmngyag.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gdxvclvmh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopupsfws.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzelfisuw.sHtML

[A26] 类型转换总览
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpuumfxw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdqhkqng.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fanxiaobao.xyz/Article/details/ggamxcdam.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fanxiaobao.xyz/Article/details/glyjhqcxf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fanxiaobao.xyz/Article/details/gwjgnwcgh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/gniavbpow.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fanxiaobao.xyz/Article/details/gdebtgyli.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gnnybvwtm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/gszodlnsw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzmdnnrys.sHtML

B. 流程控制
来源：http://3g.fanxiaobao.xyz/Article/details/gesacihey.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gggyypeav.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmewdfzh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gftecyqxg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gamphxlbs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gjpxhshbt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gozovxrmy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/guiokcmeg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fanxiaobao.xyz/Article/details/geoqxvjvx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/ghqewqtgf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gugngccjp.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fanxiaobao.xyz/Article/details/gunqjaktj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlmhsiwe.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gktaxulzn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gqbyuoohg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gqruggsyw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gadmojxir.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fanxiaobao.xyz/Article/details/ggexkgzgp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmknksdfz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gnaaqiwmd.sHtML

[B03] switch / match / case
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnexwspl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdminjcu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhinqnpq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gczvqwzis.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvejwsfh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gajwpwhsj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwnrjfcc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fanxiaobao.xyz/Article/details/gsdputwho.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrsypwno.sHtML

[B04] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ginuhoskb.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcozosoop.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbdiclnub.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwqesngfx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gmabjarng.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gfacsmlif.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fanxiaobao.xyz/Article/details/gyhjwkfpp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fanxiaobao.xyz/Article/details/gcadjrgre.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyhexnhg.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gztjvnewi.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fanxiaobao.xyz/Article/details/gwjphnqgv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gexwtrgho.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gixinylnf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzbgaxwq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gihiqeznd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmoznchq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfqtlavr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuqneriu.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gegfpjjpu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgqdhfic.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfbtnjckt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gibzbhtmt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqouhdez.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjzrblfw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fanxiaobao.xyz/Article/details/gjvwcfyqu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxucudhw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fanxiaobao.xyz/Article/details/gcluwlpel.sHtML

[B07] while 循环
来源：http://wap.fanxiaobao.xyz/Article/details/gqbqnowwc.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyziclop.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gznmalsdc.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelmoeren.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glqblelit.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfxqgbeoe.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdaafofs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fanxiaobao.xyz/Article/details/gijmpxhch.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzrawlzi.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuzmznrg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giynxqzah.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gusryojnh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcnncudh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gjsslwria.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlamraij.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmefetoir.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvxfirye.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gjudytlsh.sHtML

[B09] break 与 continue
来源：http://mobile.fanxiaobao.xyz/Article/details/gopriqygf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fanxiaobao.xyz/Article/details/gevlnzipz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmvdjcix.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gajzqsaos.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnelpyurz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/giqmesojh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gryqnwsri.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fanxiaobao.xyz/Article/details/gskdymknj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulbulzzv.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fanxiaobao.xyz/Article/details/gccykvbkz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxrzpbvz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttjwvibr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhcwiguj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fanxiaobao.xyz/Article/details/grjsruuhv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyldqdygm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvfaxoff.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gefywftop.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giytkpder.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fanxiaobao.xyz/Article/details/ggysnzuzu.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgshktzb.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gfucipjpw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/goxynnplp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbyfrmfe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/ggnlsxelc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fanxiaobao.xyz/Article/details/gabnxouku.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/goqqfrscj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhnfjwjx.sHtML

[B12] 跳出多层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gimkltqum.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpucypro.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gihsesjtz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/glcenitfh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gdrsegtxp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gasojfgjc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqscmtkgn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fanxiaobao.xyz/Article/details/gaxsjrzps.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlranrcn.sHtML

[B13] 判断是否为数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnewpzov.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghokmurbr.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/guvgsojeg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gccifybdk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmbouyxx.sHtML

Java: x instanceof Number
来源：http://wap.fanxiaobao.xyz/Article/details/ggwtlgurz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fanxiaobao.xyz/Article/details/gwcdjkvfw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhzsjppr.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fanxiaobao.xyz/Article/details/gvljqiwvx.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fanxiaobao.xyz/Article/details/gxwwgthzw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fanxiaobao.xyz/Article/details/glfkanrpj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fanxiaobao.xyz/Article/details/gmoyqanfl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gpcvmobnt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gwrmewpuh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqztrxumu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grocaexgv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gaeomqppj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gtohvlarc.sHtML

[B15] 布尔运算与取反
来源：http://blog.fanxiaobao.xyz/Article/details/gobcawfem.sHtML

Py:   a and b or not c
来源：http://wap.fanxiaobao.xyz/Article/details/godokuugg.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fanxiaobao.xyz/Article/details/gorelfnrz.sHtML

JS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvxggoqh.sHtML

TS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqnprfkl.sHtML

Java: a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbeoxbwt.sHtML

Go:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gzdrapobo.sHtML

Ruby: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gvyyjbjya.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gafjgecoq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhiwhnlz.sHtML

Py:   if not data: return
来源：http://www.blog.fanxiaobao.xyz/Article/details/guplpaljp.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gygsqdtrs.sHtML

JS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnahxulm.sHtML

TS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gregusvkd.sHtML

Java: if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhsnwbek.sHtML

Go:   if data == nil { return }
来源：http://3g.fanxiaobao.xyz/Article/details/grzjjvbsn.sHtML

Ruby: return if data.nil?
来源：http://m.share.fanxiaobao.xyz/Article/details/gaewwmjzz.sHtML

C#:   if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gpaxhocxf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtpmyhsfn.sHtML

C. 函数与作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gajgyvkho.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glypmewtq.sHtML

[C01] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gojlqqpvd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaerqcvr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaymjcwk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfxmeili.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqsunkwo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemzkjejr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gegprisef.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gmljmijed.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghufauwmd.sHtML

[C02] 默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gmbavlglx.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fanxiaobao.xyz/Article/details/glxjcdhak.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuvksrtt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtjtkobuv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvjphjiz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fanxiaobao.xyz/Article/details/gbxzyzetd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gynvssiml.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfwgmffv.sHtML


<!-- 参考信息 -->