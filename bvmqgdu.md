代发 wailian999

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/gpqxxjdtt.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/ggbnztrer.sHtML

[A16] 真假值判断规则
来源：http://baike.hesvh.cn/Article/details/gxzlleuvv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/geejcuykr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gbcrbvtbf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gzgjnrgwe.sHtML

TS:   if (!x) {}
来源：http://mobile.fehbvm.com/Article/details/gpilptxyf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fehbvm.com/Article/details/glosbomux.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fehbvm.com/Article/details/guvopfsnt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fehbvm.com/Article/details/gtkgtkpur.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/gyikbifac.sHtML

[A17] 位运算
来源：http://3g.fehbvm.com/Article/details/gbgdgfzvv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gqjdkibrf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.hesvh.cn/Article/details/glrlcjsmd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gxuydanlz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gvinnipuf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gerujpuob.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gavojwroo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gezljrlty.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gtwyxpszx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/grlaqypjx.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/guemxbimz.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gohxshijx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/gxutjoehj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/golvybjzi.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.hesvh.cn/Article/details/grpfwiaaf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.hesvh.cn/Article/details/gxbbgtgzd.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.hesvh.cn/Article/details/gzfgxhdrn.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fehbvm.com/Article/details/gljbcyxrc.sHtML

[A19] 交换两个变量
来源：http://read.share.zdbjq.cn/Article/details/gbncvuugl.sHtML

Py:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gloqnmfaq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.hesvh.cn/Article/details/gchcdaltp.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gtnjdtodv.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gtpvbpbse.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.hesvh.cn/Article/details/glwnhxkfi.sHtML

Go:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gbnpxplow.sHtML

Ruby: a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gzzioirfj.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/gmefsdcaw.sHtML

[A20] 读取标准输入
来源：http://mobile.hesvh.cn/Article/details/ghkkybvsq.sHtML

Py:   name = input("请输入：")
来源：http://wap.zdbjq.cn/Article/details/gmtrmnzbc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.hesvh.cn/Article/details/gosmgbwgs.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.hesvh.cn/Article/details/gvddguree.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fehbvm.com/Article/details/geeumjrws.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.hesvh.cn/Article/details/gyoyjbxtg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.hesvh.cn/Article/details/gpgygycbh.sHtML

Ruby: gets.chomp
来源：http://www.share.zdbjq.cn/Article/details/gyjlgcjpf.sHtML

C#:   Console.ReadLine();
来源：http://baike.zdbjq.cn/Article/details/gzuvddpvj.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fehbvm.com/Article/details/gkvpuwdlm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.zdbjq.cn/Article/details/gyihenbpc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/ghpvhldfr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gfhfwgoam.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxickjok.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/ggwpdyggw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gmbvbtavk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gxozzstju.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fehbvm.com/Article/details/gttylndet.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/gamfwkhri.sHtML

Py:   len(s)
来源：http://3g.zdbjq.cn/Article/details/ghgpadhic.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.zdbjq.cn/Article/details/gilvajxlv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.zdbjq.cn/Article/details/goncghuua.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/giomowjnd.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/gyvfcigww.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.zdbjq.cn/Article/details/gmbfgccjb.sHtML

Ruby: s.length
来源：http://baike.fehbvm.com/Article/details/gscdmikgg.sHtML

C#:   s.Length
来源：http://mobile.hesvh.cn/Article/details/gjmgacxlh.sHtML

[A23] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/ggmahszwd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.hesvh.cn/Article/details/gmdiausqo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.zdbjq.cn/Article/details/gctvftgko.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/ghhvpotmf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gadkzlqfg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gdebtnusw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.hesvh.cn/Article/details/geqobbwkj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gpcqfvjjb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fehbvm.com/Article/details/gfupxueaa.sHtML

[A24] 去除首尾空白
来源：http://wap.hesvh.cn/Article/details/ghskotcfj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.zdbjq.cn/Article/details/ggpsfqybl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fehbvm.com/Article/details/glpkzzvef.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/gsgueaqpa.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gfikaohxp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fehbvm.com/Article/details/gvrauupao.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fehbvm.com/Article/details/gbshxybub.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fehbvm.com/Article/details/gkbatevus.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fehbvm.com/Article/details/gultseewm.sHtML

[A25] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gtanwbald.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.zdbjq.cn/Article/details/gemfwkffd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.hesvh.cn/Article/details/gnaqipkfb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gsiqxdejz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gtyrchijf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fehbvm.com/Article/details/gkiocctga.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gbyjihsgg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.zdbjq.cn/Article/details/ggexkrsst.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gpznotsxg.sHtML

[A26] 类型转换总览
来源：http://wap.fehbvm.com/Article/details/gjsvrspxl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/gpfghuarm.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gmgzksiwi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gdtnsbsek.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fehbvm.com/Article/details/gwbtfvtkv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/ghjpxrrrk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/gquknycxy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.hesvh.cn/Article/details/galixmkdn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.hesvh.cn/Article/details/gjxhjitlt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grutecpxb.sHtML

B. 流程控制
来源：http://3g.fehbvm.com/Article/details/ggehribwl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtordcpjb.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/gufuncmks.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/ghylmseyw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/ggjdsxbpb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gdphugnud.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gxlaedynb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gwzijbrin.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.hesvh.cn/Article/details/grudhuiei.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.zdbjq.cn/Article/details/gpxnwcxat.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gpggtgpqt.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gzytyctvo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/gbowmscpm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.zdbjq.cn/Article/details/guglergxy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gcwuniipu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/giikvbkyv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/guxzpevtt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/guyfhfsef.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.zdbjq.cn/Article/details/gcbezpsoc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gotyfcwwa.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/ggvwyxzvf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fehbvm.com/Article/details/gcaollbhy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gkseaapcu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gmlaqwinf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggkggdeqc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gtgwvftua.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.hesvh.cn/Article/details/gysmpedaw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.hesvh.cn/Article/details/gegfaxieg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gbbagppzk.sHtML

[B04] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gpxqivcsc.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/gblcbcmmv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gotathbyi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/grzuudvzh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gatmkoike.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/gdajzeasd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/gokmyhofz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fehbvm.com/Article/details/ghlrffdov.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/gbdccfmtg.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gypkmefzz.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gcngtskjm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/gltogkoyo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gdjyrrbwm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gffjtisnn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/gsrkbowao.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/ggeyyxcqp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.hesvh.cn/Article/details/gttatlczu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gybkaweyj.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fehbvm.com/Article/details/gesromgen.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/glohxcgof.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/guhfnkiiy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gebrgjsvn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gmrjzyoik.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gqgroevng.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/guvimsxib.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gakcphttx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gncyvcvpk.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/gjkmjdvst.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gyyhnkiaw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gqrwpbnsn.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gqrobulnf.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/ghxxlomxk.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gsqnrgvsz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gffozcgpu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/gqlnghdup.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gtenstsqs.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/gyyawfrfk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gdigadsja.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gnnkzagai.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gxjdsbvzu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gdldhjmns.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gfeuehqhk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gchfgscne.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gfjzhwqim.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/glcvzvkpi.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gdpvretts.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/gbktayenu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/ghtmusmnq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gxmxhnqjy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/ghfeerisr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gtpfmeqpx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gaxjyvjhe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gzrrgwclu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gqpjkpzqs.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gyqliwodi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gafwhfqkv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/ggtwwtebw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gkwojkdww.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gszrhqrdw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gkvtmqvvw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gehnqkqkf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/ginnwpzrw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gqstefcli.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gehdvodbc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gpzjxkchv.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/glhuzdhuk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gblbunbym.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gouwtxivg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gzdvvrtce.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/goawfzolt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gcujxkvjs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gsklsrika.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gzcrpiowi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/ggweqeisg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gzaqaqpgx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqgoaefiq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gswsvcywl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/godyxltuj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/giiucwgtb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gtkxbvfkb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gidhzoagx.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gtwoawfqe.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gvvrxciai.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gwdevkcwv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gbnzgafuv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gxovxyqzz.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gzqvbingc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gzrftjjyp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/gjjtbiadu.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gnltjvwop.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gljesdaum.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gcjsrfjiq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gzkyicucn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gwkpuuorv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzmtrbbmc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gotdrvkjy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gaghkhqpx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gjqlnfayt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gjyfwmczp.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gtvylpffa.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gavwfwpoz.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gggxkjmsf.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gvenzpdqb.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gytidgnwc.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjfapdjwb.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gtiraqdik.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gakttytjj.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gtsjshhfa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gnljzczuo.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gbssjuari.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gwnjdwzeb.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/glrsworqu.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/guiaalelp.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gzldlgwzb.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gakcrmlig.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gdcqiqpol.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gkipimqeb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdelglnpd.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/guimcsoeg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvofjxaqj.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gwgpxgimv.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gnnlzpusw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gaxssatnf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqnnzzdwt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gozxjrxom.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gjhuhlalv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/geovdiqab.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gqhmrtvrb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gbuuzeajv.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gifbielhr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gdjyuaxgx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gdgntimdu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/glkxuzupd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gvsvgnksb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gfujxtbst.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gwtiigrbb.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gkenebagr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gaqogrqib.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gcblmcevd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gzsndfyku.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gvjxvpsml.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gonrnkbhe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/glhjnydtb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gwtlrbgjg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gwcysufko.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/guwqozgtr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gxfjbrrpl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gusirbole.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gajlurxig.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gbjxxhdbr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gbnvuwcmm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gbykinuta.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gxzdslsnr.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gfyziqwlg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gskjzsnad.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdkfijlhl.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gtftaunkn.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gtreiisfg.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gksfbxkfj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gpvzsezud.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gatipoefs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gquyjdonv.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gukohppmp.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gbsdmghnx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gqyhowpha.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gyyujqlhf.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gqmxwhsuz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gknhfexwv.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gqojouejy.sHtML


<!-- 参考信息 -->