代发 wailian999

Py:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gbhpioxrx.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/ghuwrnein.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gnagxgpwl.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzqkwqvm.sHtML

Java: "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gjanxwujz.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gvbpqurgn.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisxqbmtk.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqffkpmho.sHtML

[A14] 注释写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gvytcuzpc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxailzty.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchrxmbye.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gsstzftmw.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/goucnmlvg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcvudzsx.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkeecxkd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fanxiaobao.xyz/Article/details/goprkjlow.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquplewie.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtafqyxr.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcxfllwd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gqbedvudl.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giygxtpbg.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/gopkcamdy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fanxiaobao.xyz/Article/details/gmqahpmad.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fanxiaobao.xyz/Article/details/gzearbikn.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fanxiaobao.xyz/Article/details/ggbopagrx.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gfmyagvur.sHtML

[A16] 真假值判断规则
来源：http://wap.fanxiaobao.xyz/Article/details/gwkigqevq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gtcuyrdwb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fanxiaobao.xyz/Article/details/gsnqnkkoi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/gxborzaos.sHtML

TS:   if (!x) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gafcdvram.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/grwetvbjd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gehgrmnjy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fanxiaobao.xyz/Article/details/gogetaizz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggseeobzj.sHtML

[A17] 位运算
来源：http://3g.fanxiaobao.xyz/Article/details/gjpmypjdf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwhpmqap.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxibxrlw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjgnekvo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/ghxoersgh.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gzalleodt.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/ggcampbfk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwggeftoj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpcqcmiq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvquficq.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fanxiaobao.xyz/Article/details/ghjbqsxwh.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.fanxiaobao.xyz/Article/details/gchtrydkh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzrnvnzy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fanxiaobao.xyz/Article/details/gybyvhkrc.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fanxiaobao.xyz/Article/details/grgeslykz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fanxiaobao.xyz/Article/details/giczrlusl.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fanxiaobao.xyz/Article/details/gnzoznfow.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuenlfgo.sHtML

[A19] 交换两个变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvjfuzww.sHtML

Py:   a, b = b, a
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhygnwln.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.fanxiaobao.xyz/Article/details/gvugqqcil.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fanxiaobao.xyz/Article/details/gsbxxfwoy.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fanxiaobao.xyz/Article/details/gihzcexob.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fanxiaobao.xyz/Article/details/gxlenswnb.sHtML

Go:   a, b = b, a
来源：http://wap.fanxiaobao.xyz/Article/details/gthsnkksw.sHtML

Ruby: a, b = b, a
来源：http://www.share.fanxiaobao.xyz/Article/details/gnakcwnam.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fanxiaobao.xyz/Article/details/givakzboo.sHtML

[A20] 读取标准输入
来源：http://blog.fanxiaobao.xyz/Article/details/gxgyadige.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxwskuhd.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fanxiaobao.xyz/Article/details/gcdajbrpv.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpvatlan.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gdrixwkun.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhrcyvlg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.fanxiaobao.xyz/Article/details/gynmlwalp.sHtML

Ruby: gets.chomp
来源：http://3g.fanxiaobao.xyz/Article/details/gqayjrpkv.sHtML

C#:   Console.ReadLine();
来源：http://blog.fanxiaobao.xyz/Article/details/gbuqbmyuy.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fanxiaobao.xyz/Article/details/gdppaqiyl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqatgnsay.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gbsmtqdvq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkckpopig.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/geujxhnlo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnhdzfjq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gisrqarsr.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmtcdsow.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrmspizx.sHtML

[A22] 获取字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdkgfnws.sHtML

Py:   len(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/greptnhng.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fanxiaobao.xyz/Article/details/gupfeynnz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fanxiaobao.xyz/Article/details/goxktqjzc.sHtML

TS:   s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gmggqtwpc.sHtML

Java: s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcljogwb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gialaqxeh.sHtML

Ruby: s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfhjjbrq.sHtML

C#:   s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvvnyotu.sHtML

[A23] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gptsylmdl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbnaprhj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbchjdlyo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzypyfqs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fanxiaobao.xyz/Article/details/gheizyzcb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkexptzwo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisskwrxt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fanxiaobao.xyz/Article/details/gtiuhgriw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fanxiaobao.xyz/Article/details/ghqndpsbl.sHtML

[A24] 去除首尾空白
来源：http://read.share.fanxiaobao.xyz/Article/details/gfajdkobi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fanxiaobao.xyz/Article/details/grizxuiix.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqfgetvk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnswrmlwq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gerrooojw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdmhnmru.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gwansrpnp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fanxiaobao.xyz/Article/details/gvevcxnpp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gptzjmlsu.sHtML

[A25] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gmaddmkmr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fanxiaobao.xyz/Article/details/guaaionvv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfirglfi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcfvzvxk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gyhwqmoki.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoyeraow.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufgbgrrk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqhnncki.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpbifpaf.sHtML

[A26] 类型转换总览
来源：http://www.share.fanxiaobao.xyz/Article/details/gcguwimey.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fanxiaobao.xyz/Article/details/gupwjxgym.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabapmccg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwitbftts.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fanxiaobao.xyz/Article/details/gqpeaeduu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghphndgbk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fanxiaobao.xyz/Article/details/gbwvihyan.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfizmfxp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoevbykw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmiumqdv.sHtML

B. 流程控制
来源：http://mobile.fanxiaobao.xyz/Article/details/gholnmhol.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbcodkun.sHtML

[B01] 条件判断 if / else
来源：http://blog.fanxiaobao.xyz/Article/details/gvvskxjqz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fanxiaobao.xyz/Article/details/gjpswoonl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gltruqpih.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpkiscpj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/glqusbdzz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gltbbqehp.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fanxiaobao.xyz/Article/details/ggqxcmdby.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbovhlxq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaocqzam.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fanxiaobao.xyz/Article/details/gsrxrsscs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fanxiaobao.xyz/Article/details/grugakvtt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmrwhnfm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzjqnzyp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gferskahz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gueenmvij.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fanxiaobao.xyz/Article/details/gsvuacosg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fanxiaobao.xyz/Article/details/gywjyrsuq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gppidjztk.sHtML

[B03] switch / match / case
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxpwover.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdhfwxrf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyhdilmc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqlaqzlm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gubizgjmb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggdxfqevu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gzzsjxpqp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fanxiaobao.xyz/Article/details/gszqhztxx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpgwoguf.sHtML

[B04] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjwjnmjv.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsgbslkd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdafrzsun.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyrakvlp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gluvtmshl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxlnqqqzo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlzbvbah.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fanxiaobao.xyz/Article/details/glmpjrklh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpagvthda.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuqyphix.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbilrcly.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fanxiaobao.xyz/Article/details/grjphojfe.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gszxlllmt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gxyihhmnx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiaiqmfh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsgaddqu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvzchiau.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvacdiipb.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fanxiaobao.xyz/Article/details/gxxoymdnp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdutgpfg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grebtvwyy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjgynebpe.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/guxugoffp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fanxiaobao.xyz/Article/details/gftrckulm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxvrhich.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fanxiaobao.xyz/Article/details/gzuoztvrx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoojcihh.sHtML

[B07] while 循环
来源：http://m.share.fanxiaobao.xyz/Article/details/grsaokuxc.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyoolusp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbdpwqzew.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gelxcgmse.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmhzvhusy.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbadfrvkv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gsujsyzkv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fanxiaobao.xyz/Article/details/gnklmsdfs.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizptnrrx.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/gfmmeeybx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fanxiaobao.xyz/Article/details/gcnhdoeeb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghihoicze.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gaoajmahi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/ggfjiflgd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzuvjylm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gvbjqeshx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fanxiaobao.xyz/Article/details/gubyawyej.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnusoilvl.sHtML

[B09] break 与 continue
来源：http://read.share.fanxiaobao.xyz/Article/details/gdetijhvb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fanxiaobao.xyz/Article/details/geqiftxbq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtbsislz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkqktrdei.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxfigwda.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzaqjutl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhvykuye.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fanxiaobao.xyz/Article/details/glsfdptix.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glybsfbvq.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gqukfsaha.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fanxiaobao.xyz/Article/details/gehzxgtat.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gogajdzqg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fanxiaobao.xyz/Article/details/giwywxbsf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gavnodrzr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzxtruagi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzbmsgow.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fanxiaobao.xyz/Article/details/gumwdxlvv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gozghkozm.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fanxiaobao.xyz/Article/details/gzxjzymml.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmiwlgyz.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvorllgym.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gcwvzqbus.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gvsjdrpff.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/guacjxrbr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fanxiaobao.xyz/Article/details/gizevvwik.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgeqwiku.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnepjynle.sHtML

[B12] 跳出多层循环
来源：http://wap.fanxiaobao.xyz/Article/details/gymnjjeeg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkimbmqi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fanxiaobao.xyz/Article/details/ghyfqnkhn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebkphcrc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxgyyfoi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gymscfegg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkhghzktb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxicxlrib.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fanxiaobao.xyz/Article/details/guoywzfdy.sHtML

[B13] 判断是否为数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnnczcje.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyrolgex.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzoypznp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gechivhaa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gcmaexdti.sHtML

Java: x instanceof Number
来源：http://blog.fanxiaobao.xyz/Article/details/gviqxfajp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fanxiaobao.xyz/Article/details/gluclmdzl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fanxiaobao.xyz/Article/details/gbwvwbnhf.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvdujcrg.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxrlfrss.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fanxiaobao.xyz/Article/details/gjisirzec.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsckazvon.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gjzrxwhyh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gackmkyjt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpwaauyi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlndzhlf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocougrza.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpakeyfn.sHtML

[B15] 布尔运算与取反
来源：http://baike.fanxiaobao.xyz/Article/details/gyknqbfhn.sHtML

Py:   a and b or not c
来源：http://3g.fanxiaobao.xyz/Article/details/gazaolgcj.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghduirxld.sHtML

JS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gayzctxqg.sHtML

TS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gahpnnliq.sHtML

Java: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgguirpm.sHtML

Go:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/guissmaxw.sHtML

Ruby: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpbyojmb.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gwajlabuy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbiiamut.sHtML

Py:   if not data: return
来源：http://3g.fanxiaobao.xyz/Article/details/gobxjfvlj.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmnxxydt.sHtML

JS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpobaxzd.sHtML

TS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/goccinqrq.sHtML

Java: if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbanmlskf.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gvpvzzazu.sHtML

Ruby: return if data.nil?
来源：http://wap.fanxiaobao.xyz/Article/details/gxufqxzsz.sHtML

C#:   if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gduwvrrhp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfooqjznb.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gmwqvzbyh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpwzbmiu.sHtML

[C01] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwthspoy.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gcpcepzny.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grjexxcop.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqcvshtj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwriegqmv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpwfvvkl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gucunutqm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fanxiaobao.xyz/Article/details/givbrwevr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guplvavpq.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerwmogsr.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fanxiaobao.xyz/Article/details/gaatpixnv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gncaopyao.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbghbsrtr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnlfummih.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvizsphsk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grdbekgph.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fanxiaobao.xyz/Article/details/gqyreietg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fanxiaobao.xyz/Article/details/guomrlhhz.sHtML

[C03] 可变参数
来源：http://blog.fanxiaobao.xyz/Article/details/gjwzaqpow.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxswhwfxw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fanxiaobao.xyz/Article/details/gfglalfye.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gummamfcv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmmnzpti.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geblkjluy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fanxiaobao.xyz/Article/details/gzhhbeedm.sHtML


<!-- 参考信息 -->