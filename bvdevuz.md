代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.hesvh.cn/Article/details/gypmuancr.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gzgxhccrx.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gdgbwyred.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/gftjfjbex.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fehbvm.com/Article/details/gawdvucqd.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/gvpdtxzvi.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/gomzcomxm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/gtndxtkhh.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gewlkhtan.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gcskpsogt.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gkskxhzoh.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gghhqdjow.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gvqrtsrwq.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gidfckeus.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gmetylnwl.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gyajjpfjy.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/gtyovbsdh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.hesvh.cn/Article/details/ghixriwza.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/giwqjcdwo.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gwmhmhjuh.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gopfckemj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.zdbjq.cn/Article/details/gmiirpnrh.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gxstzcpov.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.zdbjq.cn/Article/details/gpzrmdjod.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gntpdrkav.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gzokjmapy.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gdgxdhqea.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/giehjcojw.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/ggfcnkfwy.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/geclsbknx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.hesvh.cn/Article/details/gyqbgacdl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/gxbzqodci.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/glmreygmf.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gixanaziy.sHtML

[A16] 真假值判断规则
来源：http://read.share.hesvh.cn/Article/details/ghdlnqtod.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/gfprliyzk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/gggezarqv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fehbvm.com/Article/details/gvoiosocc.sHtML

TS:   if (!x) {}
来源：http://www.share.hesvh.cn/Article/details/ghuacahsi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fehbvm.com/Article/details/gglrmyvyq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.zdbjq.cn/Article/details/gourrbosn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.hesvh.cn/Article/details/gcnkbonoi.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcjrfsvks.sHtML

[A17] 位运算
来源：http://3g.fehbvm.com/Article/details/gaswhozyq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gjgcrxhfc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gqkpkzlpb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/goipbwbqr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gkrebulon.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gpmqbaoel.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gguqmwldq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gdmgrqomz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gjnlgeurh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.hesvh.cn/Article/details/ggzpqvzar.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/giqjdoygq.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gwivyhurb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/gfavpzutl.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/grueqcktm.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/gatoehfrk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.zdbjq.cn/Article/details/gvfwmarmc.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.zdbjq.cn/Article/details/gfkiigrxc.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.fehbvm.com/Article/details/gmjxgujsn.sHtML

[A19] 交换两个变量
来源：http://3g.zdbjq.cn/Article/details/gqybkaljv.sHtML

Py:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gbgmjgduo.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.zdbjq.cn/Article/details/glqflhppq.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gikrtolwt.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/ggruqpjxk.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.zdbjq.cn/Article/details/gyaoyaynm.sHtML

Go:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gxugxlexy.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gcxqkhhkn.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fehbvm.com/Article/details/gduhhfeqe.sHtML

[A20] 读取标准输入
来源：http://wap.hesvh.cn/Article/details/gvbsjyjvr.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fehbvm.com/Article/details/gcrampher.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fehbvm.com/Article/details/gnabiakdn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/gtdbrflcb.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/givoimpnd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fehbvm.com/Article/details/gyerluvho.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.hesvh.cn/Article/details/gwxxjivky.sHtML

Ruby: gets.chomp
来源：http://www.blog.hesvh.cn/Article/details/gfohwtoho.sHtML

C#:   Console.ReadLine();
来源：http://3g.zdbjq.cn/Article/details/gsgworhjy.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/gmnjknjnj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fehbvm.com/Article/details/gwmtidveb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gwofyafpm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gasjphxpm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gumnpzejx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gacyueltf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gthztgxaj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gqdwdswlj.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.zdbjq.cn/Article/details/godnaytsf.sHtML

[A22] 获取字符串长度
来源：http://blog.fehbvm.com/Article/details/gluxxlnrd.sHtML

Py:   len(s)
来源：http://www.blog.fehbvm.com/Article/details/gnnxrxhyk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.zdbjq.cn/Article/details/gjyknnrtn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fehbvm.com/Article/details/gczosjwkt.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/gcchicdkz.sHtML

Java: s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gysdrigog.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.zdbjq.cn/Article/details/grodkkcdy.sHtML

Ruby: s.length
来源：http://read.share.fehbvm.com/Article/details/gyqgoctcm.sHtML

C#:   s.Length
来源：http://baike.fehbvm.com/Article/details/gecyubofb.sHtML

[A23] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/ggvnbkmiq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.zdbjq.cn/Article/details/gfwmcpsey.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/gmezuvjtp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gebcfshxw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/godfdlklu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gbspnbbtc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gjffetbyw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gcnlfeler.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fehbvm.com/Article/details/goaskwowz.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/ggoxusjsa.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.hesvh.cn/Article/details/genrglzxg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.zdbjq.cn/Article/details/gicywldef.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gopkcbjyp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/ghxyhtzej.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gsqwzwzpq.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fehbvm.com/Article/details/greqtpqwr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/gfrnvfprl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/glaqbliov.sHtML

[A25] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gmuwkbanq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gwccqtmih.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/gshorwdfr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.hesvh.cn/Article/details/gpqypfvwl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfurxnqhh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.zdbjq.cn/Article/details/gywchqusq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gidpkiqyr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.zdbjq.cn/Article/details/gjksefwqu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gimkrxrqe.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gwgnafwtj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/gmfwwkxhf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.zdbjq.cn/Article/details/gzqfgqprb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gyggsvalg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/gdqmvnlmb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gttnnvqzs.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fehbvm.com/Article/details/gdwpgpfku.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.zdbjq.cn/Article/details/gomqdvtws.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gefktdvsz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdgeyuhij.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/gxmtezjyp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glezcwwua.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/gtpoksxmh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.zdbjq.cn/Article/details/guccgthox.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.zdbjq.cn/Article/details/gjjkzcmxv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/grrtbobfo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gmkyskrok.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gmwjuzqzc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/gbaqjwsxl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fehbvm.com/Article/details/gzrjdajub.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gmpwxlsst.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gjiquhcxe.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/gxkwpbfew.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/guzskabpz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gdvybyerk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gcgkopmuy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gslcjitox.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/glekcuyha.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/ghrvltdfc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/giyfrqpjf.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gauaqjkfl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.zdbjq.cn/Article/details/gpsxcngem.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gbistyyrx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/grgrbqsfh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/ghoytuxbm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gwvlpidxk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/glwmlabdz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gstmifdjg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gcpvzfpqk.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gcnvkwvwu.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/gepmzxrpm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/gybaumbmr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gvertwwye.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gnnuxnidh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fehbvm.com/Article/details/griohprql.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gwojloxhq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/gzvltpngd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/gwfmwiedr.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gccyxgwtx.sHtML

Py:   for item in arr: print(item)
来源：http://wap.zdbjq.cn/Article/details/ggsrazqnn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gyyocnlmy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/ghyeneanp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gkeeiktwf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gzxrjsasv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcekhlxzq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.hesvh.cn/Article/details/gusuzyscn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/gpoyoscve.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/gpczwguzj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gxbnhbijs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gwxpfpyna.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gyuneykel.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gqbgmjbmg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/grpmnaztt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/giugxkwvk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/garinsppg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gafobzxtr.sHtML

[B07] while 循环
来源：http://www.share.zdbjq.cn/Article/details/garrrptqc.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/gtwjirkug.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/gavzenjqd.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gbbeelgwi.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gbnjwqyhz.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gfwpzaxxw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.hesvh.cn/Article/details/gujipujuc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/ggoaxurgr.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gcmwvfsoq.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/ghdukqcyd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gukugqbmk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gyhdyjpes.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gzsbpvwsd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gjkkesmmy.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gzejupyzt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fehbvm.com/Article/details/gfngvzbvn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gzsxijbkk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gjjcfcoab.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/gnoymgpjk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/gyonwgozn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gdvdadykh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gulonkhdo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gffqkmkdm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gyftkxehr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/grfadhzxg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/gxjvfxgqy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gdtqlzjdq.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gjlatumtc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gpowpxbnp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gtulrmvte.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gjlnpuxiv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/govasejfk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gxopcwgeu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/grdjogben.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gpftkrkyr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gqxgmumpm.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gtqmjplea.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gmpjaoqlr.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gtmngijlv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gqhokyjhc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gjiavgxzl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gdhiknxxe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/grmxopcsv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gzdhbploi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/ggwouocfc.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gogihajxb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gihgeoxgt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/grmrpquqd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gzzrzgwbf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/giwbmakjm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gzvmovwzx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gbnihhwcc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gyufbnxvw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gczfgevaa.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gscoktnul.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gokgqzmtn.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gwkwmwgiz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/galprjuxz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/ghupiexbt.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/glkwwlopz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gcsxrunbu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/grgptkazk.sHtML

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/gomxvqzpb.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/goptyhpom.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gnjutsghk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gfdjdnpil.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/ghhfhfprp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gnhjtrjoi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gkeimpvkf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/gchfetkyl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gtkymdbpz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gtbeounxb.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gzeewopka.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gjumudjrd.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/glqrnjsjh.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gpwylgvgm.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gookihexa.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/glouztbjh.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gieebufaa.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gsvuqskhz.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gykumyyxo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gyjgscdwq.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gzieyjxoi.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gjrtjkxvt.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gusxbxkzx.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gclguyfty.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gkuqxjzri.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gnqznkumt.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gmbtleyxm.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/glxrcmcyy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghklzectk.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gpfwlpyzc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpqijnvyw.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/grufiejpq.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gjdxmmszq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/ggznhaotx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/glvwwzhpl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gdccilkul.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gdpnczlaj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gestztyky.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gssfjaaro.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gxlptvjwd.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gwgqgadzs.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gdqtgsilz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gqfoyxthj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gtzwdfflz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/guwsyfyxm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gzarxsonb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gvufdpgyz.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gorvexjkv.sHtML


<!-- 参考信息 -->