代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgkxrdqy.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprjmyysv.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfvoydee.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqptiovqp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjilzwzg.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhmwlbay.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glexylvde.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fanxiaobao.xyz/Article/details/gvbjujpup.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gyiueclwo.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gnnsaueck.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgtryxen.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsjquxjg.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gexwqdxnb.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gncertetw.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gircslsrc.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxrrnoxb.sHtML

[A14] 注释写法
来源：http://3g.fanxiaobao.xyz/Article/details/gucieykpz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fanxiaobao.xyz/Article/details/gxwlfnnqk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpdonjob.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtqylync.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gmojpspmr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fanxiaobao.xyz/Article/details/gpuglexqz.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gxygdhdof.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fanxiaobao.xyz/Article/details/giklfftzh.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gtssyeaap.sHtML

[A15] 空值判断与默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gdynsqrfe.sHtML

Py:   value = data or "默认值"
来源：http://3g.fanxiaobao.xyz/Article/details/gyzamtpwn.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gchtuweno.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufiovbor.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gfajyazaa.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkrtwrxv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwybhwag.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fanxiaobao.xyz/Article/details/gsycntyfy.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/gevsrstxm.sHtML

[A16] 真假值判断规则
来源：http://mobile.fanxiaobao.xyz/Article/details/gftpmvlyi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfrvvqsr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fanxiaobao.xyz/Article/details/gusspmqau.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiilswpn.sHtML

TS:   if (!x) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gixztilcc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjohndnqz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkceruhnb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/gjsinsllb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/guauzfcao.sHtML

[A17] 位运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmhntpab.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjoqvtry.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/ggdzfxzoq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gpoaqbcuw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gcusvnjmv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkcsflvu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzfxoslz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsagpkii.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuujrvfs.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswreoxxw.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gqwaoltxn.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gltbfmypg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fanxiaobao.xyz/Article/details/gradlltyi.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gmyjzovnv.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmbrrdxf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.fanxiaobao.xyz/Article/details/gsenmhuyv.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fanxiaobao.xyz/Article/details/gfgcotxpb.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjknzgfy.sHtML

[A19] 交换两个变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gccjjnxgx.sHtML

Py:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmabfhru.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fanxiaobao.xyz/Article/details/gtnlnimkc.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxvrupsw.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fanxiaobao.xyz/Article/details/glzgteptm.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fanxiaobao.xyz/Article/details/grwvxavoq.sHtML

Go:   a, b = b, a
来源：http://wap.fanxiaobao.xyz/Article/details/gzbganhnj.sHtML

Ruby: a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/gglztxfef.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gofyyauzy.sHtML

[A20] 读取标准输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gajodrpvr.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fanxiaobao.xyz/Article/details/glumyedni.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnavokchn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fanxiaobao.xyz/Article/details/gtciepufv.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gxqzwppnt.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrijrwnm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fanxiaobao.xyz/Article/details/gbjfrcxgj.sHtML

Ruby: gets.chomp
来源：http://mobile.fanxiaobao.xyz/Article/details/giwiwmmfj.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fanxiaobao.xyz/Article/details/gnumgdldk.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/getbqgkfj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghvmclgeg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfmcwwib.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpjgpsoh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfopdwhku.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggomdlhzd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyycgofe.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fanxiaobao.xyz/Article/details/gsosxojvo.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fanxiaobao.xyz/Article/details/gfuwxbhsp.sHtML

[A22] 获取字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/guuxthpjv.sHtML

Py:   len(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgudhekq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fanxiaobao.xyz/Article/details/gqrrlnjvs.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fanxiaobao.xyz/Article/details/grukoazip.sHtML

TS:   s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gtypntkmt.sHtML

Java: s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpjyqqxa.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwttcxbel.sHtML

Ruby: s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gchijwlxo.sHtML

C#:   s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxhqyijs.sHtML

[A23] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmtsthby.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gluxjerrk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvwnoflo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gdbhpwbtj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/gotibkvat.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gpgsobdiq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gozwpsxln.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/grwylietf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fanxiaobao.xyz/Article/details/gztuqupcp.sHtML

[A24] 去除首尾空白
来源：http://baike.fanxiaobao.xyz/Article/details/ghwadphve.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnczbkzu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fanxiaobao.xyz/Article/details/glkkojrna.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbnepklr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gknysznja.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fanxiaobao.xyz/Article/details/gukxcjiyg.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzxyvopv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fanxiaobao.xyz/Article/details/gyomgluqe.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gantoeydf.sHtML

[A25] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gdixxoeeu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fanxiaobao.xyz/Article/details/gdnumyoks.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gclkjxdtj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmtymkid.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gurcuxuqs.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjkllqexw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gptkwrkvs.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fanxiaobao.xyz/Article/details/gdokigemr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpqdqrzt.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchktkkng.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fanxiaobao.xyz/Article/details/gangyojdk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxyeuztu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gursjkidq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjpjetgg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbjksvud.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fanxiaobao.xyz/Article/details/gjcpfpsiu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fanxiaobao.xyz/Article/details/ghqweqngy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/gehydohkb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvgaejaho.sHtML

B. 流程控制
来源：http://blog.fanxiaobao.xyz/Article/details/gwhbbdgkh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkeclvsvh.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fanxiaobao.xyz/Article/details/gliazshdh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbupnjyb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzmhshiy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/glqsrqnca.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gbwdmrzvf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gngxazfzw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfbqdeme.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/gasoulywj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gofwiowka.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fanxiaobao.xyz/Article/details/gormtjooa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fanxiaobao.xyz/Article/details/gjpklgsmj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glrktvfwx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugfcqgmo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlkowgpt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvptarjzu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gweopdfyq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fanxiaobao.xyz/Article/details/gcfxnvokm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczkemngj.sHtML

[B03] switch / match / case
来源：http://www.share.fanxiaobao.xyz/Article/details/gmagqvqan.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fanxiaobao.xyz/Article/details/gpetenoty.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gitwzydkk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtabvgnxv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcifbuxv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsytksyhu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoknavdk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvxxbxfv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gfoxrvlww.sHtML

[B04] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnnzjgtg.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxxiyfux.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrliwbhy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/guzakgdhq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjtdneov.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaglxebbk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqmgrbdh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fanxiaobao.xyz/Article/details/goaogzoal.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmftbcoe.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgmjhxjk.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fanxiaobao.xyz/Article/details/grcawuvwq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyjfwqyl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcxmvyti.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvyiauaxo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geotwnqki.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fanxiaobao.xyz/Article/details/gybnhyyxf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fanxiaobao.xyz/Article/details/grajqkhfs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqbodlhsb.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gamkmcjnk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycfcyoez.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gscdtijao.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwddrlanr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzspauno.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmhtownt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhfkksao.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fanxiaobao.xyz/Article/details/gnmkeqcda.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/glyfzmhhl.sHtML

[B07] while 循环
来源：http://blog.fanxiaobao.xyz/Article/details/gsrhaepjn.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gbchowymh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtenzykk.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gipuwzrae.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gktumvwwp.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzldtoybz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gmobqduas.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fanxiaobao.xyz/Article/details/gpszlmprs.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzooedyhm.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fanxiaobao.xyz/Article/details/glcghgkvb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fanxiaobao.xyz/Article/details/gpuwhmbza.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfotlffgw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gigwrvzcl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdxujsre.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdnutbmj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcmbucim.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fanxiaobao.xyz/Article/details/glqbrjqwm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gezxfzdkp.sHtML

[B09] break 与 continue
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfakumpev.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/gnnuwbjbc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiuvzlkx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giaxmgosi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgtzgvbv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gobokwjjz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gceamkmya.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzorrtqc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glvyptmza.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gsepudlof.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fanxiaobao.xyz/Article/details/gvlvspqal.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgmfpzyp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gehzkwcnd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/guacpoxol.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfixddfub.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gwkphtevw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtglppucd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/gnxopjmbq.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwmzbzpi.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fanxiaobao.xyz/Article/details/gwxgrykjd.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gubqahnmk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhbefeik.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapnbidhl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gyegrtdge.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguxbnfar.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsmrqnox.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gconqoigi.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvkfjgpn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fanxiaobao.xyz/Article/details/gqpdtrbkj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmrxmpnr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gyfqyxkpr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnfykqwb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gawutewkk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fanxiaobao.xyz/Article/details/gttofydln.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvftphqa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fanxiaobao.xyz/Article/details/gxczpsrfk.sHtML

[B13] 判断是否为数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlacvffg.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscypwnxx.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsfxvkcy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gocflitek.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/giqawjyoo.sHtML

Java: x instanceof Number
来源：http://mobile.fanxiaobao.xyz/Article/details/gtevkayob.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvzbalpq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjfvukxc.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fanxiaobao.xyz/Article/details/gaykrdqys.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwudnxqb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fanxiaobao.xyz/Article/details/gjyvfavsp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbdtsqrx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxavzxrzu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwdncnwg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gxcmbiqwi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gidcyotop.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gbhpjlvei.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvymmagvc.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/glllleuqe.sHtML

Py:   a and b or not c
来源：http://wap.fanxiaobao.xyz/Article/details/gavwtsbeq.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxeiwohg.sHtML

JS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/ghblxdljc.sHtML

TS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnqakbsi.sHtML

Java: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmnybywa.sHtML

Go:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gnhbocmpl.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwpblfxf.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gnupdmnhr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/ggrkouxvx.sHtML

Py:   if not data: return
来源：http://3g.fanxiaobao.xyz/Article/details/gezpiddln.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaovdzhqy.sHtML

JS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvyctmjo.sHtML

TS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gazvftvqe.sHtML

Java: if (data == null) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkflixco.sHtML

Go:   if data == nil { return }
来源：http://baike.fanxiaobao.xyz/Article/details/glstxsevt.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtsdqupm.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gypsfnrtv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/geukdnkpu.sHtML

C. 函数与作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdstkoefh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggcqaqxxs.sHtML

[C01] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdhzwtzr.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gjpgmfrig.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtouxnmub.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbpyzanf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpvrsown.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoiytreo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnpjvxvw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fanxiaobao.xyz/Article/details/gpxoecmrl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdpiqpwtz.sHtML

[C02] 默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuqhtiyy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlvpmsjr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnudcxswo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqnvgnhfb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwlozmpsk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fanxiaobao.xyz/Article/details/geebckdli.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fanxiaobao.xyz/Article/details/glsdvlqmp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtgjqcfb.sHtML


<!-- 参考信息 -->