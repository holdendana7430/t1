代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gobqzlhcz.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fanxiaobao.xyz/Article/details/gsigdemcl.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gossllhwg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gywqavldd.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gnlhupirv.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepteuuzd.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fanxiaobao.xyz/Article/details/gxrdhvuwq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fanxiaobao.xyz/Article/details/gxjwwpzir.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gbjdehusy.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkyhztuw.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gnffjedhp.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabkhksoi.sHtML

Java: "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gqrogosvo.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtmqykdi.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthhohmks.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynzrvayu.sHtML

[A14] 注释写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoomtqru.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexilfdkr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboulniix.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgqnrcij.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gifqljiyh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gaufhwndj.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubsjhjyc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fanxiaobao.xyz/Article/details/gapnjbzpo.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gesdoeqoh.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvvocaor.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdfrjfay.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gkgobbqwb.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gjwcuubta.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gknmfcqog.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdxsnnro.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyprjufcx.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjergwmj.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gzegllakh.sHtML

[A16] 真假值判断规则
来源：http://baike.fanxiaobao.xyz/Article/details/gdzfrfdzc.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpcuplyx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxbiiwlr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghipnbzrl.sHtML

TS:   if (!x) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gafsvbfig.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gajtwjsza.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gaosvxvxe.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumnsvgkx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gsolmgpvr.sHtML

[A17] 位运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrdffvek.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlljdtzg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqnbcnya.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshfrqhrq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gtdnyorlz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsldrxuwk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gohslfqnr.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gefzfyjds.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gglnhprqj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fanxiaobao.xyz/Article/details/glqraniaz.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxsymubt.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdawwdsjo.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkugtajk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmavrwjx.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fanxiaobao.xyz/Article/details/gvndfpfag.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fanxiaobao.xyz/Article/details/grtrdqakq.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fanxiaobao.xyz/Article/details/gdsfsjocs.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.fanxiaobao.xyz/Article/details/gzyjrmnph.sHtML

[A19] 交换两个变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqvrbgqdm.sHtML

Py:   a, b = b, a
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlmqbmok.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfratnctu.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddkdikiq.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fanxiaobao.xyz/Article/details/gsoxrwvdt.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fanxiaobao.xyz/Article/details/gcxibygnv.sHtML

Go:   a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/gheewsbxq.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpljmhth.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fanxiaobao.xyz/Article/details/gktgaorfz.sHtML

[A20] 读取标准输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gndbckrte.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goibdjvjn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgyvpjdj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fanxiaobao.xyz/Article/details/gbxitfefr.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrjmrzfl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmnmmluv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fanxiaobao.xyz/Article/details/gjcacjyql.sHtML

Ruby: gets.chomp
来源：http://read.share.fanxiaobao.xyz/Article/details/gwogvwzwq.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmlryvtx.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gplcgxrna.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsrktfyp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giicvnhcf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtggkemxc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gkiqohopu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghewzxpim.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.fanxiaobao.xyz/Article/details/gaatmvkym.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gkdzcwohf.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkegkkdex.sHtML

[A22] 获取字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gezrrkhqw.sHtML

Py:   len(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynhluhot.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fanxiaobao.xyz/Article/details/gpqpribjz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqqykblu.sHtML

TS:   s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gguzgwuxm.sHtML

Java: s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcqogxwx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjglucyte.sHtML

Ruby: s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhwkzimt.sHtML

C#:   s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdfuhkdv.sHtML

[A23] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gshuaigsg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fanxiaobao.xyz/Article/details/giztuvqio.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fanxiaobao.xyz/Article/details/gdtogqcxp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/gttnwlcva.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fanxiaobao.xyz/Article/details/gjmkorhcd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/giqsvilxh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gjtkibfwo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fanxiaobao.xyz/Article/details/gchremtvf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqufhxdt.sHtML

[A24] 去除首尾空白
来源：http://blog.fanxiaobao.xyz/Article/details/guylteiop.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fanxiaobao.xyz/Article/details/gxyxyewxa.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fanxiaobao.xyz/Article/details/grvbektpo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnivvuxd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwsxttaw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgzjsxor.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdquzuaan.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fanxiaobao.xyz/Article/details/gcimorfqm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/gggytgmck.sHtML

[A25] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogydvafq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgwpfufg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvbmaffz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/galjshfxf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkyqraexl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gerfldhqj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fanxiaobao.xyz/Article/details/glsjjfyfv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fanxiaobao.xyz/Article/details/galisjufk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gudcoyeiq.sHtML

[A26] 类型转换总览
来源：http://baike.fanxiaobao.xyz/Article/details/gnplpywen.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fanxiaobao.xyz/Article/details/gavcnndbo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fanxiaobao.xyz/Article/details/gijgergty.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fanxiaobao.xyz/Article/details/gdckoovuj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjtjfoby.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fanxiaobao.xyz/Article/details/gfyojdkgr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaebgoapp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gdlhkoayh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqmokmgj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlduguwt.sHtML

B. 流程控制
来源：http://blog.fanxiaobao.xyz/Article/details/gqkrvsezj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/getrokqed.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fanxiaobao.xyz/Article/details/gucxkplgx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/grorvllng.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyyfigod.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/grqqsnnir.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guprtbsct.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gxtoiqiak.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gryztcmhs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvixjcwao.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/girldqqux.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fanxiaobao.xyz/Article/details/gcavmatvb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fanxiaobao.xyz/Article/details/grppqifha.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxedfhtrd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gdfmcfawj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gukyzspru.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/gynlkziwe.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fanxiaobao.xyz/Article/details/grignsotk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fanxiaobao.xyz/Article/details/gisavvssu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzetowvc.sHtML

[B03] switch / match / case
来源：http://blog.fanxiaobao.xyz/Article/details/gwkoanrgf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginubrhrm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtganixuj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaecsgwcr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkgpeejkw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnpktqfs.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrykxnpz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzbrquyu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkavafkf.sHtML

[B04] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxkmazlp.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gojtymrhj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxnpujxdb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gapgkusyp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvlzerwcw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzshoibe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzogwymc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fanxiaobao.xyz/Article/details/glypmgyps.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyoelqqs.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gszjplrze.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkctvuyqd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnblurmv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfcorrzf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/ggxxobegn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gmdklbgzy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyqvtbtk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fanxiaobao.xyz/Article/details/gfmahpwbk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdjffeqk.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gupgozwtq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fanxiaobao.xyz/Article/details/gvlztxnnp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gccosoren.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbzbyxlkp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gallsyehg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fanxiaobao.xyz/Article/details/geqarmuba.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdabvqphb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fanxiaobao.xyz/Article/details/gjmrcjlnd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtumlgeoc.sHtML

[B07] while 循环
来源：http://3g.fanxiaobao.xyz/Article/details/gfuxbypdz.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fanxiaobao.xyz/Article/details/getmwlvrj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtfapiwhj.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqosxfgie.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gszkuitqy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjaatpsn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fanxiaobao.xyz/Article/details/gdyngcdoi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzrlsxrv.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdtixffm.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrzguoxr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvchelykh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/giaygstrp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmakaaguu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguzdoygm.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gkrpizadg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fanxiaobao.xyz/Article/details/gircetxdn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpmaikks.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gmqdbpkpi.sHtML

[B09] break 与 continue
来源：http://read.share.fanxiaobao.xyz/Article/details/grgtuwkpf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvficogi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glzasycuw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gevbciooh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjizqqnx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/guwnlknaj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/gtyuhobxx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnemswvba.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjqxubmvd.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmzaxdju.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fanxiaobao.xyz/Article/details/guqosrryd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fanxiaobao.xyz/Article/details/grkjmvron.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fanxiaobao.xyz/Article/details/gegpnqgrh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyvhfgsr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fanxiaobao.xyz/Article/details/gpxjryyqs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gooplhlbs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fanxiaobao.xyz/Article/details/giatodfpi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/geboodixg.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fanxiaobao.xyz/Article/details/gdvdlznoe.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fanxiaobao.xyz/Article/details/gzhflllvw.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcxamqiw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gueaxtpyd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdxkexlk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gndqwzhsn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fanxiaobao.xyz/Article/details/grkvsxvfx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gvistmgek.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gugfehqcp.sHtML

[B12] 跳出多层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/geyfoidrb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmuehbpu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fanxiaobao.xyz/Article/details/geadphazv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtswpbuos.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/grcrefhtj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfpiqtqd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoyuzyvd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fanxiaobao.xyz/Article/details/gbsgzmtrc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxqsehbf.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gjjtaftav.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fanxiaobao.xyz/Article/details/gqtoazcfx.sHtML

PHP:  is_numeric($x)
来源：http://3g.fanxiaobao.xyz/Article/details/gbwueksfm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/ghayxeltl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gnyuhhydo.sHtML

Java: x instanceof Number
来源：http://baike.fanxiaobao.xyz/Article/details/gwacdxtmk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwscvrbaz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopovandl.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fanxiaobao.xyz/Article/details/ghttlmgdl.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fanxiaobao.xyz/Article/details/gkwvuabdl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fanxiaobao.xyz/Article/details/gnitrgyen.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fanxiaobao.xyz/Article/details/glfslmvpy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqdhzjpv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/guhcqhpgm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsisbying.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueevypfl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griktoeeb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gexnllcfy.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtqiloeh.sHtML

Py:   a and b or not c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzpacckb.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fanxiaobao.xyz/Article/details/gntpmqhpc.sHtML

JS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/guimwuzle.sHtML

TS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgspxhat.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gkieoxbca.sHtML

Go:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gycddmkcq.sHtML

Ruby: a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gugwivrvy.sHtML

C#:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtiyhpur.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/geqzzsawu.sHtML

Py:   if not data: return
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxirjhqq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gebzkovqx.sHtML

JS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcwvvino.sHtML

TS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gijwfjnfa.sHtML

Java: if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gxlpatude.sHtML

Go:   if data == nil { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gksmfevyv.sHtML

Ruby: return if data.nil?
来源：http://baike.fanxiaobao.xyz/Article/details/goxhhbekt.sHtML

C#:   if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gifobarof.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdujyjvld.sHtML

C. 函数与作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmihortm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxupxvtuc.sHtML

[C01] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqmmvyla.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfugskqmt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqftwedjt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwxuegoz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glvrpzjjg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajgxbrtf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gygryxedh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/grihnsrcm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjwbnkbt.sHtML

[C02] 默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsawthdcr.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fanxiaobao.xyz/Article/details/gclxeonrv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/giznwkflv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxugvrhcl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmgagaqbq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftkayazj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fanxiaobao.xyz/Article/details/gawjflxyx.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyeecuje.sHtML


<!-- 参考信息 -->