代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/gcanosxcn.sHtML

[A11] 条件表达式（三元）
来源：http://blog.zdbjq.cn/Article/details/gkhzwpcku.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fehbvm.com/Article/details/gzvvtkpip.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/grazqslfv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gfnfrdfsj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gkodfnshx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gjukyoapg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/gqdyjicep.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gxnvhlbku.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/ghjgkyqzi.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.zdbjq.cn/Article/details/gwnvbxnkx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/gozrxcjkj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.fehbvm.com/Article/details/gevxnlcyu.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gpenlbndc.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gtvlgehet.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/glcceyaak.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.hesvh.cn/Article/details/ghcugkyrq.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/ghytnmegu.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.zdbjq.cn/Article/details/gffberzfx.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/gmydkeicd.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gdsvowjpr.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gojmporvh.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/ggjpepmua.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/ggmzruuht.sHtML

Java: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gkveiwrhb.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/ggkqbqtov.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gyhyxhgzp.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gpimpramm.sHtML

[A14] 注释写法
来源：http://m.share.fehbvm.com/Article/details/gemkxckkh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gheshjxlz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/glgezxvwf.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/grtxbecwn.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/ganfwwoxh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/gmwtkkbtc.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gowclysvn.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fehbvm.com/Article/details/geniarcsz.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gjpbdcyfb.sHtML

[A15] 空值判断与默认值
来源：http://baike.zdbjq.cn/Article/details/geqvgumbe.sHtML

Py:   value = data or "默认值"
来源：http://baike.hesvh.cn/Article/details/gxubtsnup.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/giilantbr.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gtywfrvpl.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/ghpmwwnfi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.zdbjq.cn/Article/details/gywdcffux.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.hesvh.cn/Article/details/glvaftcbq.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/gzjcaxnqq.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/goihnhwbt.sHtML

[A16] 真假值判断规则
来源：http://mobile.fehbvm.com/Article/details/gmckjijav.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.hesvh.cn/Article/details/grgjaeczg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fehbvm.com/Article/details/grurmhmrh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/gheahdqmc.sHtML

TS:   if (!x) {}
来源：http://www.share.zdbjq.cn/Article/details/gvkzphvcf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqhajuneq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.zdbjq.cn/Article/details/guctupljh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fehbvm.com/Article/details/gqcqlcvpw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gmntpdxle.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/gblojfkoa.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gaqbylsgc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.zdbjq.cn/Article/details/giilgjmaw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gkvepnnsf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/ghomwaayj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gtdydzlvn.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gsrdwzydd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gjbshldds.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/glnpmibcl.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.hesvh.cn/Article/details/giubjqgxc.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gvgzlixgy.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/ghlceprvo.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/gddkuzlzx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gcngvpeax.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.hesvh.cn/Article/details/gshftwiny.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.hesvh.cn/Article/details/gkuakagjo.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.hesvh.cn/Article/details/geanjwvem.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/grjzmmheb.sHtML

[A19] 交换两个变量
来源：http://read.share.hesvh.cn/Article/details/glitcvgqe.sHtML

Py:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gkffiyfsy.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.hesvh.cn/Article/details/gjmqegncm.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/ggnfckyga.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gxwdqxikk.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.fehbvm.com/Article/details/gccqldrov.sHtML

Go:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gutjhivko.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gokebntsz.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fehbvm.com/Article/details/grnqpfpxu.sHtML

[A20] 读取标准输入
来源：http://m.share.zdbjq.cn/Article/details/glsvfgpbt.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fehbvm.com/Article/details/gpjzlgqit.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.zdbjq.cn/Article/details/gketngvgy.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fehbvm.com/Article/details/gljzctjeb.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.hesvh.cn/Article/details/gzcbtmxbk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.zdbjq.cn/Article/details/giznjynwf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fehbvm.com/Article/details/goenqutnq.sHtML

Ruby: gets.chomp
来源：http://read.share.fehbvm.com/Article/details/gurnugcrm.sHtML

C#:   Console.ReadLine();
来源：http://mobile.hesvh.cn/Article/details/gpdrozdyw.sHtML

[A21] 保留指定小数位输出
来源：http://wap.hesvh.cn/Article/details/gtklzkpah.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.zdbjq.cn/Article/details/ggbddagcz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gatzdwscq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gstdxqyhu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/geiagiolj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gmvzcxtrc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gbphyjggx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/giemvyujl.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fehbvm.com/Article/details/gvrysrvvp.sHtML

[A22] 获取字符串长度
来源：http://www.share.fehbvm.com/Article/details/gqofcmwhu.sHtML

Py:   len(s)
来源：http://mobile.zdbjq.cn/Article/details/gnfkyrxtt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.zdbjq.cn/Article/details/gbrflgpzl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fehbvm.com/Article/details/gvtceqddu.sHtML

TS:   s.length
来源：http://blog.zdbjq.cn/Article/details/gjrqcxpci.sHtML

Java: s.length()
来源：http://www.blog.fehbvm.com/Article/details/gsaemegdz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fehbvm.com/Article/details/gmyndqpao.sHtML

Ruby: s.length
来源：http://wap.hesvh.cn/Article/details/ggjmzhvlp.sHtML

C#:   s.Length
来源：http://blog.fehbvm.com/Article/details/gysekgquz.sHtML

[A23] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gaxljkqsu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gtnatbfcc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.hesvh.cn/Article/details/gpybbenho.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gqyrxjzhc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gwybydsrj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gltqsnbrw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.zdbjq.cn/Article/details/gjiviiltk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gqvbbfypc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.zdbjq.cn/Article/details/gnzyzoydp.sHtML

[A24] 去除首尾空白
来源：http://www.share.fehbvm.com/Article/details/gvhdjkjay.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.hesvh.cn/Article/details/gmfbeyqjd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.zdbjq.cn/Article/details/gmcyooitj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gsquoommq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gwpgwuqnh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fehbvm.com/Article/details/gjkkaelox.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.zdbjq.cn/Article/details/gaaenmtvr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gnutjfwfy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.hesvh.cn/Article/details/gcggwedfr.sHtML

[A25] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/geqqmdwor.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gtmvfcano.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fehbvm.com/Article/details/gorimlbsp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gkxzccqhk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gvcxpkhyf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/gledrnrte.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gmlfukdop.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.zdbjq.cn/Article/details/gltznqjmx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gttgwhtik.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/gjpslebaf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.hesvh.cn/Article/details/gskbturfz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/ghmyfqgmo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.zdbjq.cn/Article/details/gemhhvnkq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fehbvm.com/Article/details/gxjmqzsye.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/glatxjxmu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fehbvm.com/Article/details/glxxdyjyt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.zdbjq.cn/Article/details/gebxawqxi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gpgjpryio.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gctjobkja.sHtML

B. 流程控制
来源：http://read.share.fehbvm.com/Article/details/gqsxgimec.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grslcjdkw.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/ggdtwmamg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/gixaijvte.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.hesvh.cn/Article/details/gxqlttiem.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gorxrsubv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gidqsyigm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gysiytxwc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.hesvh.cn/Article/details/gbscexcrl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fehbvm.com/Article/details/gmxnkjvbe.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gdxhywjlr.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fehbvm.com/Article/details/gvitxsbup.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.hesvh.cn/Article/details/gprgswfnq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/gtaqirkvm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/ggzoshpav.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gdikyiwxu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gntwieudl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/gepeclrsm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.zdbjq.cn/Article/details/guysrgvwz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gmzaiisfy.sHtML

[B03] switch / match / case
来源：http://www.m.share.hesvh.cn/Article/details/grhlabgdq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gymhlzwsr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/ghdmtxufa.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkyyawyna.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gmdwxzjqi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gmhgqskxq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fehbvm.com/Article/details/gbylitdqo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gkdswqnck.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gochtfxxx.sHtML

[B04] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gfrvcqmtg.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gmqawasgl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/gaetlkmlt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gsqsyolvn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gacfdffry.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.hesvh.cn/Article/details/gocgckbwm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gnzszfstm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.hesvh.cn/Article/details/gogpcjpko.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gsasknoel.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gztamkore.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/ggxwjynya.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/gzqgvubpl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gzqgvjvot.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/goyumnnon.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/gcucmdecw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gwepvfqzt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/gytdsqwlh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gngcuswdw.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/griodmwzm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gykuguxyo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gorkfyywm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gdfpfcgza.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/geeficunl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gupnblzkd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/ghqfjkucx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/glzicyxio.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.zdbjq.cn/Article/details/gfxfsehbl.sHtML

[B07] while 循环
来源：http://read.share.fehbvm.com/Article/details/gyltckqgl.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/gtcoodioc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/ghrgzjhvc.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gndhahoyl.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/grfgugxoh.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/ggmhudksr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/glpmsckju.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gasubmlno.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/ggetwyidy.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/gliohpbmw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/gqywiwnpv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/gwmjforkr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/ggyluchqm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gjpxknlbo.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/grfveexwp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gimtpajwn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gcjtgsems.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/ghurypdqh.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gqqbplbmc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/gxzqnkoqu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gvorqnvex.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/ghinphkba.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gfwcqmbai.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gycpkimbq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/ghrgkoghi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gdyifetqv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/ghzkxnnsm.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gzoppatae.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.hesvh.cn/Article/details/gszaesmok.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/ghiwahcii.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/goxgicvqv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gkgnqydns.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gwqfatxiz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gvaacncnd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/glvddfpdb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gyyuohsby.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/gelgyxccj.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/ggbrrkqtv.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gltajiebo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/ghsyizwhr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gyrrxlyqc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gvvncdexo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gqwdsiqxj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/grwssejex.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/giipjeejt.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/ggjiyludm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gdxmutmhc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gwwketwby.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gupqllzqs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gttpixpnj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gbihsacfz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/ghpfzhguq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/ggormqvbv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gpldyqvln.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gkwxuzzgo.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gyeshfutc.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gbqipeeok.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gfnyrsxkb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/grneorhfq.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gdwdnzjnk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gvioepxek.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/ghrpnguha.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/ggvldjnwl.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gjalrnmla.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gxkzcqvpe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gugeeszba.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gijjzehpz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gjyadcwyx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjvljirmg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gqmznricn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gugfrxkvd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gdpbjjsbl.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gkbwmcgmn.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gqhooyxqb.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/ggdlkzpik.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gkmjrfpce.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gvvxpjxkv.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gzjyrplxr.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/ggrsefuhu.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gmmjwjlfo.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gkycsmqpk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gztzomluz.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gpbpxtnwz.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gwwojnuab.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gtjqualum.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gmnzofhxj.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gnfcnjfzg.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gywaezgoc.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gpetofieg.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gmeqvlcqs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghlaagcnl.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gpcjkbhnl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gffrejwmv.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gavnmgkzt.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gouycoysc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gxvbraone.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gxzpnrngu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gzzppkdph.sHtML


<!-- 参考信息 -->