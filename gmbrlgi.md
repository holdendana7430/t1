代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gpgnrnohv.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gctwxdgri.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/geewiymbu.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/glpbmnjrw.sHtML

Java: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gfaoobvdw.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gnssabmqf.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gfuhjazai.sHtML

C#:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gugjhhxgn.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/gkutehkhd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/gqvscmulw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/giphxdedr.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gcrvxkywm.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/grslcookv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fehbvm.com/Article/details/gcmsluyyg.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/grehulytf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fehbvm.com/Article/details/gjsidzxcw.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/ggrvotehb.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/gpssccleg.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/gvvkadxrz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/giwxziydn.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gofbmpxzj.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gsctumnkn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fehbvm.com/Article/details/glvloivjz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.zdbjq.cn/Article/details/gigmmguns.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/gawgobabc.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gzeyhkvlc.sHtML

[A16] 真假值判断规则
来源：http://www.share.zdbjq.cn/Article/details/galjidrhf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gvpcmjlsc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.zdbjq.cn/Article/details/gytkrwkwx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.hesvh.cn/Article/details/gpnuwbedc.sHtML

TS:   if (!x) {}
来源：http://mobile.hesvh.cn/Article/details/gyaavonmh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fehbvm.com/Article/details/gnnwkdpds.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fehbvm.com/Article/details/gwcqceumi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gkxjayauf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.zdbjq.cn/Article/details/gbyjliqmn.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/gpglsngiv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gevgdiwub.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gzqinudxi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gtrlctvdh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqxuczsaw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gsepuoado.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gkdjfqime.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gvknolzdl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkdchnbcw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/guerdpgry.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gqmmmmapk.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gyvibctyz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/gwkgodwwd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gdiedyalr.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.zdbjq.cn/Article/details/guzvbgzmz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fehbvm.com/Article/details/gehrsxppx.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fehbvm.com/Article/details/gxfidoemx.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.hesvh.cn/Article/details/gboenabpk.sHtML

[A19] 交换两个变量
来源：http://read.share.fehbvm.com/Article/details/gdoxseqjz.sHtML

Py:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gobzccrsz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fehbvm.com/Article/details/gzytwmxmu.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gwhmoxtgr.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/gipkzclpp.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.hesvh.cn/Article/details/gwrwtirkw.sHtML

Go:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/grzbndodb.sHtML

Ruby: a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/ggediqijf.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.zdbjq.cn/Article/details/gwxyzfxjr.sHtML

[A20] 读取标准输入
来源：http://baike.hesvh.cn/Article/details/gcrvhibio.sHtML

Py:   name = input("请输入：")
来源：http://m.share.hesvh.cn/Article/details/gbrwfhfwi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.hesvh.cn/Article/details/gfobcgylh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.hesvh.cn/Article/details/glfjceiif.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gadquruvl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.fehbvm.com/Article/details/gojsinnza.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fehbvm.com/Article/details/gpcwkatps.sHtML

Ruby: gets.chomp
来源：http://wap.fehbvm.com/Article/details/gjtoynzuu.sHtML

C#:   Console.ReadLine();
来源：http://blog.zdbjq.cn/Article/details/gwcmztuua.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fehbvm.com/Article/details/gaxftmrdj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fehbvm.com/Article/details/gwqkxgssg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gezgywxql.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gipcgsetc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gdnwlwluf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/ganzwnygx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gnavomreq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gdiefkbog.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.zdbjq.cn/Article/details/gvkstwcuv.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gupaekalp.sHtML

Py:   len(s)
来源：http://3g.hesvh.cn/Article/details/gwstvyscn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.hesvh.cn/Article/details/ghxxiolir.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.zdbjq.cn/Article/details/gwbeieuls.sHtML

TS:   s.length
来源：http://www.share.zdbjq.cn/Article/details/gcpzcqpnc.sHtML

Java: s.length()
来源：http://baike.fehbvm.com/Article/details/gbvwtnkjq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fehbvm.com/Article/details/gtttjwswv.sHtML

Ruby: s.length
来源：http://blog.fehbvm.com/Article/details/gevtlaadb.sHtML

C#:   s.Length
来源：http://read.share.hesvh.cn/Article/details/gcaqweibl.sHtML

[A23] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfwfjiwvz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fehbvm.com/Article/details/gsbvicjlo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fehbvm.com/Article/details/gyzueazad.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gcguyfjlb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gwjwocrva.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gvxeizzyl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gsllcacgt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gnlivokmu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.hesvh.cn/Article/details/gvijopaym.sHtML

[A24] 去除首尾空白
来源：http://wap.zdbjq.cn/Article/details/guwrtwsal.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.hesvh.cn/Article/details/gppqiiaao.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.hesvh.cn/Article/details/gkqvwhdup.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gfxdkfgih.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gdrpgkzsb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.hesvh.cn/Article/details/gwohpezci.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpvwbgqiu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.zdbjq.cn/Article/details/gvthqnlhv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/glzuchuni.sHtML

[A25] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gjujbknoa.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fehbvm.com/Article/details/ghavvoieg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.zdbjq.cn/Article/details/gifbnebkh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/glnjrecdl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gzbaqmzee.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.zdbjq.cn/Article/details/gwsoiahcl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gucthllgn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.hesvh.cn/Article/details/gvknoevbn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gljdguumt.sHtML

[A26] 类型转换总览
来源：http://m.share.hesvh.cn/Article/details/gngdjkdwb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fehbvm.com/Article/details/gjfuspfeu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gdgnouvox.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/gtgdfasmd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.zdbjq.cn/Article/details/gyrsoorci.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.hesvh.cn/Article/details/geolaoaeh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fehbvm.com/Article/details/gklnmajew.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.hesvh.cn/Article/details/gkgvtpzck.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gadfprpye.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glrykwetg.sHtML

B. 流程控制
来源：http://www.blog.fehbvm.com/Article/details/gxxvqsgzl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glexbrscc.sHtML

[B01] 条件判断 if / else
来源：http://3g.hesvh.cn/Article/details/gaexdwxce.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.zdbjq.cn/Article/details/gtzffhldc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.zdbjq.cn/Article/details/gdrhwahhk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gbpkpglza.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gpkeyvink.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gjxlmitrd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.hesvh.cn/Article/details/gaxwacttg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gkyrpqnjo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gemweylhr.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.hesvh.cn/Article/details/gzlybcxtp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/ghdmzhlkt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.zdbjq.cn/Article/details/gousmkmoz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gruyyznaz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gceeqbsxz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/ggtmoloub.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/guzaqohki.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.hesvh.cn/Article/details/gjaxjulsh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gdeusrtcy.sHtML

[B03] switch / match / case
来源：http://www.m.share.hesvh.cn/Article/details/ghubgmfiw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gmnsnagkx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqaqksyck.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/giwfykage.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gqixmoczz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gshjhsrgb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gvchccgpf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gaunrdvwa.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gllharkbn.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gdmhfgsyd.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/glbwjajvu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gmrlpprqj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/ghuxqyjnr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/ggvgabidk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.hesvh.cn/Article/details/gorlkgwrd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.hesvh.cn/Article/details/gkfurmlva.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.hesvh.cn/Article/details/gponjklin.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/gryhmacsc.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gceassmio.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fehbvm.com/Article/details/gxjybdglk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/glhqixycr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gzjkiwxhm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gqawisgyh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/giwgarwso.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/ghrsmyqtr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/gcbiowoda.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/gkaghcojs.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/ggegazdgp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gdkbrrusf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gxmkijsda.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gwrifdypd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gxnfxjtvm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/ghkxigguw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gpptlwxvo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.hesvh.cn/Article/details/godekjemw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/guhwqsnwv.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gkocpqjvp.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/guziugtyy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.zdbjq.cn/Article/details/gkzdukili.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gtbrstvfq.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/guxfgsrla.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gmqybyivb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gzfrocfxx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gujgqvwbr.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gxgrqnppy.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gfsyojvqu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gvkmmdvgd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/groaaskhb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gbkkuomuh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gdzeukznp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gdyvlhmdl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gbliwfakd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gardvesmh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gesmcwceu.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gpupfrujy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/ghiwnbyyp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/goiwqsyvo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gceoohrcu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gkjzxnhda.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gdfzhzbre.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gjwiuogdq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gvfrmnhny.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gfkjouflb.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gxljbgmjm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gtpbirvtf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/gpnzqhpjs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gqldhjnph.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/guwcusggu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gfoiibwxm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gvnrfvzan.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gxbahxyyh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gteggobsd.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gomxbcfsb.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/ggzkeofyu.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gezwpjigj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gvftrrzwc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gatqyqtyb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gxzaxdsrc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gcyidlkfz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/grocjodys.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gkzamfgjd.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gjcewjyph.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/govtarupg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gkdolqdvv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gpzptjpxw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gwwckgpih.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gwzaswrov.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/glsslffgs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gczczpyos.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gdstgszwh.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gokbzutmz.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gkresqldf.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/ghnlzemfs.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gsnlgnhpk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gcrzhrayl.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gblxzsxii.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gbofwyhvm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gaeauednb.sHtML

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/gdabfmray.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gbvpyvysn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gfgbiydjj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/geonsyzra.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gbbgqebip.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gqntmkeka.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gljcbgjpx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gzcnqtpsn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gmilihyca.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxjthbikn.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gdfbbadxq.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gtgisotwf.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gwgntvxyd.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gfgblemwk.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gdroqczkh.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gvrargefh.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/grghnfaij.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gdrrwospc.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gpcjbjvpa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gnqwwvpkk.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gnttdjgtr.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gcpjdfmxo.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gmbqismul.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/ghsjpidtn.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/guivpnpnl.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gwlcbahsw.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gnkmehqgl.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gxlypbugf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guyifieid.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gaoiwbwmc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpvlaphrj.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gebhzyxfq.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gltgnsene.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gtevltipk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gapddsnop.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gfrgwvien.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqtfwkuqf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gzgssqngc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gebtenanu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gzebvzdvn.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gffstvztd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gjuajcxie.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzrjzyoej.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/goomnwovu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gcexdpcfq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/ghxlhobjf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gteuhrwim.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/grmdpwxws.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gqtwnkmrp.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/guwburdab.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gipmftiuf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gndmzafno.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gqqxjjcgr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gojxpmuox.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gfqtzsicc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gcvdqdytt.sHtML


<!-- 参考信息 -->