代发 wailian999

[A14] 注释写法
来源：http://blog.fanxiaobao.xyz/Article/details/gdiygupwp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthnpsqrc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gntjifnjh.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/glvmyzdob.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsjmbmqt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmllmnmpu.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjpulhbg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpkxbwow.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/ggtuvgigp.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdqwesqh.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsoxjnav.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gjmbnztqc.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gigfchjfm.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gkwykghsd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fanxiaobao.xyz/Article/details/gahgfeqho.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtngunvrx.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmynkrip.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcoljvkx.sHtML

[A16] 真假值判断规则
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcahgqmw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fanxiaobao.xyz/Article/details/gzzuewbtx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fanxiaobao.xyz/Article/details/gliogdgka.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfmivcda.sHtML

TS:   if (!x) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjbmtwzvs.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gkskdntne.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fanxiaobao.xyz/Article/details/giorxroam.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fanxiaobao.xyz/Article/details/grromojdw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqtspkyt.sHtML

[A17] 位运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gispdjgss.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmjxfopc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gubeveizz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjkjprrc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gfihpnols.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gbmfremjl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gibedtawc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/ghyzhlkgv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gvywktrll.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjjskgdb.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/glfofvrph.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/gevmxfktj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gewtyfdmd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fanxiaobao.xyz/Article/details/ghnsswvhy.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fanxiaobao.xyz/Article/details/gnozltehf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fanxiaobao.xyz/Article/details/guyhjadvt.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fanxiaobao.xyz/Article/details/gekwoscrd.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulofxvrt.sHtML

[A19] 交换两个变量
来源：http://baike.fanxiaobao.xyz/Article/details/glvekctym.sHtML

Py:   a, b = b, a
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbvinjxe.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzogiqir.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatwkerky.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqdtijrj.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fanxiaobao.xyz/Article/details/gdtddpeey.sHtML

Go:   a, b = b, a
来源：http://3g.fanxiaobao.xyz/Article/details/gsjmxbirw.sHtML

Ruby: a, b = b, a
来源：http://wap.fanxiaobao.xyz/Article/details/gdhlnnoej.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvamagok.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqlukzej.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fanxiaobao.xyz/Article/details/geubhjqlu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlvnpdez.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fanxiaobao.xyz/Article/details/gbjntvpwt.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/gsowwfgyl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuwmifvq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fanxiaobao.xyz/Article/details/gzpxygfko.sHtML

Ruby: gets.chomp
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfmbezhj.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhrxvtuy.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fanxiaobao.xyz/Article/details/gowdjtqdu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpxglzvdy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwbsccse.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaxmgqvr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqadswan.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/gduoytssm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gqroyrxvs.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxjsukfo.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fanxiaobao.xyz/Article/details/guxegfhht.sHtML

[A22] 获取字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gssrymjom.sHtML

Py:   len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyjedqnn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fanxiaobao.xyz/Article/details/giqxadtzk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfkpbecc.sHtML

TS:   s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeypzqyd.sHtML

Java: s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmugjeoy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gttaqmvap.sHtML

Ruby: s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gelojhkiu.sHtML

C#:   s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqwmppld.sHtML

[A23] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxxsuyqf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gtvsvckof.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwqzjhlt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmexosmif.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmfqucnm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrveuubg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fanxiaobao.xyz/Article/details/grvnkjijw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fanxiaobao.xyz/Article/details/gvdqslfbm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fanxiaobao.xyz/Article/details/gyploduid.sHtML

[A24] 去除首尾空白
来源：http://blog.fanxiaobao.xyz/Article/details/gfzvjmjxo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fanxiaobao.xyz/Article/details/gipvodahh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgmpugwb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbjyufrw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gubyaverp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxypqgqrh.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gviemhjub.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtetniqox.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gevfxhssr.sHtML

[A25] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcufabtq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhzneire.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtaicweu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gnbnbeblc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwglqqbm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksubxazt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fanxiaobao.xyz/Article/details/ghwvllskk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyacogig.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpykfyoh.sHtML

[A26] 类型转换总览
来源：http://3g.fanxiaobao.xyz/Article/details/gqlmscfiu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxiraupk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyihmnzf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnlhojqm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fanxiaobao.xyz/Article/details/gfiwflgbw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fanxiaobao.xyz/Article/details/gudohlmob.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkbnosnv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgrfqoqn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvvqnljs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwegibbl.sHtML

B. 流程控制
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjeroqiy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywhdvsou.sHtML

[B01] 条件判断 if / else
来源：http://blog.fanxiaobao.xyz/Article/details/ggrjodmva.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsioratq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gthgvuhif.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwgefewq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggguzffqh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gtgohdfdc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwlktwqd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnassatpd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gsraujifo.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtudupmef.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fanxiaobao.xyz/Article/details/gixqxiyho.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqojdgvc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypnofioq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtymsytt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gthdroutw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fanxiaobao.xyz/Article/details/gtnzwamjx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fanxiaobao.xyz/Article/details/gwzhzwluo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gkckxcqil.sHtML

[B03] switch / match / case
来源：http://read.share.fanxiaobao.xyz/Article/details/gafmkpiff.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fanxiaobao.xyz/Article/details/gthhmzhgc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmroypgtk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gulquyivc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwvwiikl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gacfjygvr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpjjqvfk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fanxiaobao.xyz/Article/details/goxinsjvh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gchwvutyl.sHtML

[B04] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gcgtjprpt.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsufzelrf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmknfrzhs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbxhpwnby.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/glotcedmp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkvmlhppk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnewpvdim.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzukfapx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzprbjdj.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxdjimqi.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fanxiaobao.xyz/Article/details/gofyopnbw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzcbclzd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbhbhwxd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggorprlio.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/grndzytaw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fanxiaobao.xyz/Article/details/gwnqcsunb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fanxiaobao.xyz/Article/details/grumcvujz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtecsrfal.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeivkgnf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyhbwpjw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwmzedji.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gefftglfv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fanxiaobao.xyz/Article/details/ghehdxzdl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxomrtorv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsoecplq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fanxiaobao.xyz/Article/details/grjfbfrro.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gwimepnof.sHtML

[B07] while 循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gowcqlrgb.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fanxiaobao.xyz/Article/details/grdqoufrs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbjiyvke.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsmberrg.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqxmctykt.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnhooqjin.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fanxiaobao.xyz/Article/details/gapdbmcjn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdkgzkrx.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqxrhfgj.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/ggmtvxegi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitfhduko.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gnntghbnx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzugvprto.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvrphejy.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfdpfvcd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/grglcljqd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjtjxnkk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/guxcxffgb.sHtML

[B09] break 与 continue
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpjqyfce.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fanxiaobao.xyz/Article/details/gchdjjezt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzekhvvjw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/goudegejo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gruheaseq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmocerxw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gofsbvnpz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhgqnwvz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwppufpey.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gknqjexsz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fanxiaobao.xyz/Article/details/gqeacljjk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnbyxyhn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fanxiaobao.xyz/Article/details/gizgnpypw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/gjrxfamfh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gusewfbsy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/geyjgqzns.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhhcpkoo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggozgvjcg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fanxiaobao.xyz/Article/details/gfipewmbc.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fanxiaobao.xyz/Article/details/ghhhzhppg.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfkddubn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyklnlqfy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gwxauwyje.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gepftysfv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakduwrvd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gcvzdllhf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gyghtkbxt.sHtML

[B12] 跳出多层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gocdayavc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fanxiaobao.xyz/Article/details/glhfcnlsu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpzvdcwk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/grkpfcivb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdjbsmsk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznvnjftr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fanxiaobao.xyz/Article/details/gncawwpup.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeivrvvd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fanxiaobao.xyz/Article/details/gkslaoyhc.sHtML

[B13] 判断是否为数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtfxtvki.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fanxiaobao.xyz/Article/details/gdnapwhxg.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmwfyilg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvjrjztu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/geyrkdstq.sHtML

Java: x instanceof Number
来源：http://www.share.fanxiaobao.xyz/Article/details/gpujqqiky.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fanxiaobao.xyz/Article/details/gujbpwquo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fanxiaobao.xyz/Article/details/gsmprhwwa.sHtML

C#:   x is int or double or decimal
来源：http://wap.fanxiaobao.xyz/Article/details/geaqbxyxi.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmdimsvm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fanxiaobao.xyz/Article/details/gciihdgnc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnutfatb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gmxtkpskz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdhuqvyt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqddrsza.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fanxiaobao.xyz/Article/details/glxehtfjz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gggosnyfw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gekwnvjno.sHtML

[B15] 布尔运算与取反
来源：http://3g.fanxiaobao.xyz/Article/details/gckxkfhfx.sHtML

Py:   a and b or not c
来源：http://3g.fanxiaobao.xyz/Article/details/geqbvlfim.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fanxiaobao.xyz/Article/details/gpoiscqbz.sHtML

JS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfjheioj.sHtML

TS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxpbkikt.sHtML

Java: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gykupuutv.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsolkqsad.sHtML

Ruby: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gbiyfdlyq.sHtML

C#:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gfxauolsq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzczmxoeh.sHtML

Py:   if not data: return
来源：http://read.share.fanxiaobao.xyz/Article/details/guoyjqoga.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjutjtgly.sHtML

JS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwihdkyzn.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/ggmfeckab.sHtML

Java: if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gsgznriqg.sHtML

Go:   if data == nil { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gwvtkhrxw.sHtML

Ruby: return if data.nil?
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlfrfsas.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiqldypa.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqiszeuw.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gtlikktul.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grmdrmxtk.sHtML

[C01] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/grzoixcvg.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzjruzou.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/glyfbkvdn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiopmtfm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gazsqqsey.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbkmgvdfm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gliziwofv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fanxiaobao.xyz/Article/details/gjpeamcbk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjmzrpsbw.sHtML

[C02] 默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/godjfncql.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfqnesqj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghqkmofcz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaknytjl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxnrlmnzk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fanxiaobao.xyz/Article/details/genhssnjd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaendmyi.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fanxiaobao.xyz/Article/details/guxshdnsb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fanxiaobao.xyz/Article/details/gzdwlzjoa.sHtML

[C03] 可变参数
来源：http://baike.fanxiaobao.xyz/Article/details/gcttbrihn.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fanxiaobao.xyz/Article/details/guqdciqzl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghemwgkfj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkwltcwnd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgebtsii.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gefmyovaa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fanxiaobao.xyz/Article/details/gxqfkdrto.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdaasmbg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmffpcoa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/gourdgnhn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fanxiaobao.xyz/Article/details/gfeibavcl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gofyoyngd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfkswwewg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fanxiaobao.xyz/Article/details/gormdfsuf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fanxiaobao.xyz/Article/details/ggcpkmsse.sHtML


<!-- 参考信息 -->