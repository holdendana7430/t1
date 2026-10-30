代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/gizcszudb.sHtML

[A11] 条件表达式（三元）
来源：http://3g.zdbjq.cn/Article/details/gpoteqjod.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.hesvh.cn/Article/details/gsphebmfq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gkdbabxfi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gwnpxfjvy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gerozufan.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gucukfzcf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gjwkfpcbt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/giypwdpol.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gqhrwclgo.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.zdbjq.cn/Article/details/ghtcvpkmm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/gvhqhevcp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.zdbjq.cn/Article/details/ghlrdbxsl.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gjuabqico.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/gewkfniaw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/gvhxionus.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fehbvm.com/Article/details/gvwomqjne.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/gsmqhvsic.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fehbvm.com/Article/details/gsbhmtaud.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.zdbjq.cn/Article/details/gnadyiphu.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gpgbyvmrb.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/grirdclfl.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gkacnjqub.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gdbdwabhw.sHtML

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/geiljgwfc.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gcrcfpwen.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gcwaqlzps.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gmusvczxo.sHtML

[A14] 注释写法
来源：http://www.blog.hesvh.cn/Article/details/gtsqiqsdo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gxlkivoiu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gedurrqgh.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gbtihiqpj.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gatkslasc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gacwpdekk.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gumwybmfn.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/ghjgpxsqk.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gtpchsycb.sHtML

[A15] 空值判断与默认值
来源：http://3g.zdbjq.cn/Article/details/gjgscafnu.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/grrqjuoul.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/grrczxkgu.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gkqxdfohq.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gkuhmjzou.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/gficswogs.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/gffmlntbv.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gywsqblth.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/guywbulnm.sHtML

[A16] 真假值判断规则
来源：http://read.share.hesvh.cn/Article/details/gmyfqtdus.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.zdbjq.cn/Article/details/gjjasymrs.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.zdbjq.cn/Article/details/gijatwmyy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.zdbjq.cn/Article/details/gsbsiekyc.sHtML

TS:   if (!x) {}
来源：http://read.share.fehbvm.com/Article/details/gfjrcsmyv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.zdbjq.cn/Article/details/gdcfvqcil.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/gmbjujjbr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gyatbvciy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.hesvh.cn/Article/details/gxhavkxqz.sHtML

[A17] 位运算
来源：http://3g.fehbvm.com/Article/details/gwbweydhg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gsqjcjgrv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gufryqskq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gqjzlqnej.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gtcsajahq.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gjhsxiyex.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gnqvmnbmm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gsvldbuhh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gyusjzkvu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fehbvm.com/Article/details/gjcdlnguj.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gwyamzdzt.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/glsiisrma.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/ggmjmwqpf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gfrhgrhqq.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.hesvh.cn/Article/details/ggydrixpk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fehbvm.com/Article/details/gjxbrczzs.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.hesvh.cn/Article/details/ghchrucwg.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.hesvh.cn/Article/details/gwrdikgpd.sHtML

[A19] 交换两个变量
来源：http://baike.zdbjq.cn/Article/details/gymlqglau.sHtML

Py:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/grgehzgod.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fehbvm.com/Article/details/gsoegyzor.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gycoxyrnh.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/gsiokijyf.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.zdbjq.cn/Article/details/gauexwaid.sHtML

Go:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/goywnqtca.sHtML

Ruby: a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/gjagqlvzw.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.fehbvm.com/Article/details/ggptragtu.sHtML

[A20] 读取标准输入
来源：http://www.blog.zdbjq.cn/Article/details/gvfswkqzu.sHtML

Py:   name = input("请输入：")
来源：http://blog.zdbjq.cn/Article/details/gzbzapgev.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.hesvh.cn/Article/details/glnsfuqdc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fehbvm.com/Article/details/gilogwmin.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.zdbjq.cn/Article/details/gjhjodpuj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.hesvh.cn/Article/details/gpditwbuu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.hesvh.cn/Article/details/ghztalnvn.sHtML

Ruby: gets.chomp
来源：http://read.share.fehbvm.com/Article/details/gdeldeqql.sHtML

C#:   Console.ReadLine();
来源：http://baike.zdbjq.cn/Article/details/gbxsqwsbu.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/gghtkulzh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.zdbjq.cn/Article/details/gqmjbzzad.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gosaempki.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gncqkkzhz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gviiqlnvz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gsahlrddc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/goizvffco.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gbwdrnehj.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.zdbjq.cn/Article/details/gdyvmxwiw.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gruxwswbw.sHtML

Py:   len(s)
来源：http://3g.fehbvm.com/Article/details/gxjrsxbrk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.hesvh.cn/Article/details/gqqbcxkag.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.zdbjq.cn/Article/details/gklhyntwz.sHtML

TS:   s.length
来源：http://blog.hesvh.cn/Article/details/gukdjjoqn.sHtML

Java: s.length()
来源：http://3g.fehbvm.com/Article/details/gphdckwoo.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.zdbjq.cn/Article/details/ghfrhcoph.sHtML

Ruby: s.length
来源：http://wap.hesvh.cn/Article/details/gqfimuwea.sHtML

C#:   s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gdzpnbqtx.sHtML

[A23] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/grdexngke.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.hesvh.cn/Article/details/gqkmwfytv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fehbvm.com/Article/details/gtbsfbfbu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/ggremkijo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gbkiqmsab.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gyxjorsej.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fehbvm.com/Article/details/gwyzjstmz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gakxvlyhd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/greeylwoh.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fehbvm.com/Article/details/gzhypxdfr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.zdbjq.cn/Article/details/gohmanxnz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.zdbjq.cn/Article/details/gbthglygc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gfclrfmjp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gfvfgrddi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gikiieelf.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fehbvm.com/Article/details/ggpqpirpv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.hesvh.cn/Article/details/gvduetwie.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fehbvm.com/Article/details/gjcpqmrqq.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/grielsxhm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.hesvh.cn/Article/details/gxlzuaxzu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.zdbjq.cn/Article/details/gphfljbjr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gckirhjww.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/gtqdjozox.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/guiqlpqij.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gnhowblhq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.zdbjq.cn/Article/details/gqfzkkymh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvyjtyhzh.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gaqhbovqz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fehbvm.com/Article/details/gprcfjqsc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.hesvh.cn/Article/details/gobcqgpzl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fehbvm.com/Article/details/gtencuwxp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fehbvm.com/Article/details/gitkolkzm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/gwszagtxi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.zdbjq.cn/Article/details/ghdfopzji.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gnefmnjgc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gvhhctusi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbmlpsyzh.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/gtfftrtox.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gslttciso.sHtML

[B01] 条件判断 if / else
来源：http://m.share.zdbjq.cn/Article/details/gxxcmvtwz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gabfcbmyc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.zdbjq.cn/Article/details/gxlzfkxax.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gcrvcsquh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gigxzxysb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gtcjgcizh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/grtanjueb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.hesvh.cn/Article/details/gjaalmchy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gtxnpehnu.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/groloomzh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.hesvh.cn/Article/details/gwkndiuuj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gaprxisfo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gbbkzhalg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gptlalsch.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gkvoozzan.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/gmovbbcwc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.zdbjq.cn/Article/details/gvjuayeov.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gerduuidk.sHtML

[B03] switch / match / case
来源：http://mobile.zdbjq.cn/Article/details/gqbtedlsr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fehbvm.com/Article/details/gxvwyuvqy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gfozliatr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gdzrrxzsf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gpljuoezm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/grtvryufx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gedlrsvfl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/grqyhndkw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gybqgyfxy.sHtML

[B04] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/grfvsopfv.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.hesvh.cn/Article/details/gczdjsjmp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fehbvm.com/Article/details/gpxekwxpg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/goefenjtm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gawydvkmt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/giniziutm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/gvzjvppzw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.hesvh.cn/Article/details/gbrjuswnm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/gquwwysjf.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gerbgbffn.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/grzbuzjam.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/gkytaecma.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/gkfvvgjnp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gkclbetma.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gxqlygzbz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/gfjrmgucc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/ghoshnfyy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gnxxzocnr.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gtfldgikf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.zdbjq.cn/Article/details/gzjvghdbz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fehbvm.com/Article/details/gqpekrijs.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gjuwzgznj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gakkuqdgf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gqenuotfx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.zdbjq.cn/Article/details/gyjccjftl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gbltsojtv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gpaglsqja.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/ggryfxpzk.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/gkeitmyek.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gwqzhadkp.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/guctvijqu.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gfwbolcjh.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gftnhcphl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/ggileuweh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/georaeppc.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gbdloguhj.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/gppnocuyb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gaklgdvbz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gbqsgmsya.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gjqxlbmge.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gpaksbcjx.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/guedpzwbj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gniqakmrt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gmzqkcaph.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/ghzjcdyhw.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/glxetwuwi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/ghtmvhoyq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gkbcagnhg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gzrbheksj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gmlvocoue.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gikyyzfes.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gtyblgxms.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gbljxswce.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gehkiqeps.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/giznksnzt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.hesvh.cn/Article/details/gbnemfpgg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gxkfbmfxy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gavyvsmpn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gpjztiqxy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/grtcfvpbz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gzqbrswlp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/goqqixsck.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gmbqsrjen.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gqsgpdlah.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gzkngurcc.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/ghihgbmfc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvrebjxxb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gvihqmkxz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gfwceqbmx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gifpsyjsk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gormyqeve.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/glzfauuza.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gmgoaifvh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gvljqvhvi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gsmxrqdmo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gcfhhnzoo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gfeglnycl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gzhukyjpu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gvbhgebhj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gyxhungvv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gopujvtfi.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gvjspojtq.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gdcdxeonw.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gtlqpscrg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gopvqpmwr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gwqadcrez.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gpnrqyeoo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gdgciafqj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/gerzqbtjh.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gchnjmoml.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gzbravpyy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gygcjvvtx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gblscnfoo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/ghugtyyck.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gczsjeucl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gqhccrnqc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gckttljeu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gkwjffqkl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gbixlaguh.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gwlqsnvyl.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gspdptkos.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gcwvsfmjs.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/glpwvuvuk.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gpplhpuvn.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gxyemkhjr.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gysxtctnu.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gslcaicxw.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gejtkgarz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/grbtwjffi.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/girudxlcl.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gmpiwnsrd.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gvkamewyo.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/grmufnrky.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/ghzlzvauc.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gbkejgwjl.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gczirclio.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gaqufonsb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtbrpgbck.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gqmcrvyrm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtjfdcfhe.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gujwuxjqc.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gcaonahhy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gvtvutpju.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/geeodylca.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gdjkndweu.sHtML


<!-- 参考信息 -->