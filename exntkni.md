代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.zdbjq.cn/Article/details/gymzvoxih.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gjqvncqey.sHtML

TS:   if (!x) {}
来源：http://www.m.share.hesvh.cn/Article/details/gngpzmdeg.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.zdbjq.cn/Article/details/geyyeonsz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.fehbvm.com/Article/details/gydlrkqdr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/gpmmdufja.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.zdbjq.cn/Article/details/ghgdxffez.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/gxfmieiua.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gkbuicvfe.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gltenokur.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gzivldaji.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gfwzjinul.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gtcxkzdad.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gvwqxijas.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gwxloqivd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gyyrjajzh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.hesvh.cn/Article/details/gxgakecvs.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gtyfuenks.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gwmiuyidq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/gvdbqsufr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gcpormbnw.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.zdbjq.cn/Article/details/gjtqgojkm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.hesvh.cn/Article/details/gejtqptsu.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fehbvm.com/Article/details/gfpvknsbb.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fehbvm.com/Article/details/geqjwutnz.sHtML

[A19] 交换两个变量
来源：http://wap.zdbjq.cn/Article/details/gmfcracjs.sHtML

Py:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gaadkzapu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.zdbjq.cn/Article/details/gslvjqron.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fehbvm.com/Article/details/gijiqavdc.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fehbvm.com/Article/details/gerjtolrk.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/ghzrjbtwp.sHtML

Go:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gjxjkywkg.sHtML

Ruby: a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/gzmfkgzkl.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fehbvm.com/Article/details/gtgxjgdoz.sHtML

[A20] 读取标准输入
来源：http://mobile.hesvh.cn/Article/details/gqrfulwee.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.hesvh.cn/Article/details/gnbiwsfgq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fehbvm.com/Article/details/gilsnnfos.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.zdbjq.cn/Article/details/gtdcniqra.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.hesvh.cn/Article/details/gdupypixz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/gbizqvxza.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.zdbjq.cn/Article/details/goqlvulzp.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gmlvzlles.sHtML

C#:   Console.ReadLine();
来源：http://3g.zdbjq.cn/Article/details/gilqbkayw.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fehbvm.com/Article/details/gxbhzuhqj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.hesvh.cn/Article/details/gorplxdgn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/glmpkyrly.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gtsmsyezm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gifjjpqjn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gnugxqkql.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/godxkxzpx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/glmgwlxtv.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fehbvm.com/Article/details/gkihwxine.sHtML

[A22] 获取字符串长度
来源：http://www.share.fehbvm.com/Article/details/gvnoynhyx.sHtML

Py:   len(s)
来源：http://blog.hesvh.cn/Article/details/gudoxyluj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.zdbjq.cn/Article/details/gfsqwurzi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fehbvm.com/Article/details/grwgmhqkz.sHtML

TS:   s.length
来源：http://blog.fehbvm.com/Article/details/gnuiynsun.sHtML

Java: s.length()
来源：http://mobile.fehbvm.com/Article/details/gfznscjwo.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.hesvh.cn/Article/details/gwlvutlpd.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/gmyacyaot.sHtML

C#:   s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gjfqmpjue.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gewqtqfws.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gdipwfide.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/gdcpuhngi.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gveuhrtom.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gqklilece.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gfakbnxkx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gazgweudd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fehbvm.com/Article/details/gsxrfdmuy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fehbvm.com/Article/details/gtykgajwc.sHtML

[A24] 去除首尾空白
来源：http://www.blog.zdbjq.cn/Article/details/glltzpzlx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.zdbjq.cn/Article/details/gqjwpmgxl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfumefmfx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gckmmbvcd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/ghpfwwqva.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gpfbgoggp.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/gkpcbakvl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fehbvm.com/Article/details/grtqfdjmu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.zdbjq.cn/Article/details/gpsexssqo.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gmhufhqle.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fehbvm.com/Article/details/gewotuycc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fehbvm.com/Article/details/ghyngrdyx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/gguvepkmj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gygkcfctz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.hesvh.cn/Article/details/gduwhjjxi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gmmnalyqy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.zdbjq.cn/Article/details/gurccizhe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gigbrzilt.sHtML

[A26] 类型转换总览
来源：http://www.m.share.hesvh.cn/Article/details/gtjhzczem.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gxqzaydej.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.zdbjq.cn/Article/details/gungbwezv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gjtycistt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gyfhcsdun.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/gxzaakskl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.zdbjq.cn/Article/details/gexfphfid.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.hesvh.cn/Article/details/gndgxcaey.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/ggwznvjmy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvxcqtkll.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/gtqqnylzr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqbsymwda.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fehbvm.com/Article/details/gigwtnxsu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.hesvh.cn/Article/details/gluhufkue.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/ggnfsounr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gkdxpdrhq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gctpqgtul.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gqzfdqfpz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gufaldraj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.hesvh.cn/Article/details/gvcqoalda.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gzqawvugu.sHtML

[B02] 多分支 else if / elif
来源：http://3g.hesvh.cn/Article/details/gfzbwtfyq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/gstkezxnq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/gkuyenusr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/genlhnozg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/grmmtkokq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/ggouflhdj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/guxqxryyx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/gpfsgcpew.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gugwsphbv.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/gjevggeqv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.hesvh.cn/Article/details/gffmauggu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gvycbjdmv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gscndbnks.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/giobdvtcq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gresdwmku.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/ganrbbqih.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.hesvh.cn/Article/details/gdjbrkxvp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gjjoqicpe.sHtML

[B04] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gwuylfisw.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gfajgtlrq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gfbpnzcoe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/grwsaeegm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gfttzujrr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/gskxgpimb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.hesvh.cn/Article/details/gcnkknait.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fehbvm.com/Article/details/gxkxlvvmy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/glafwepxq.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gpanrilbl.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gpbalupwv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.zdbjq.cn/Article/details/gnnvisbck.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gmomqjvsa.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gtzqmwtrx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fehbvm.com/Article/details/gqxevcibm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/galggfggs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/givubvvbj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gurjlesqg.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/ghekzbmpi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fehbvm.com/Article/details/ghdnwlojx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/gpbwkalej.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gvxrcacmm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gojrmdjiv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gxhajefvq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gpxlgigzm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gudmkjpky.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gyjpuolvp.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gclsstfen.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gxlrptaug.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/glvxtpgwl.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gkoqockwk.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gjsutopbn.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gqnsknxux.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gxaiplasg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/glepyjgox.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gynshvtoj.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gbdlydrqu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gbaizlblo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gzymewava.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gfdzqyvfd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gozlnflmn.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gsabbilcg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gnsbykqrl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gfnbryazx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gooxoznas.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gotuvmsbs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gukemblvs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gkrgvyoix.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gzjiokurz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gaoiozbim.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/guqsnpdrz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gidhprldv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gcprrykbi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gnoevpwkj.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/gnmziieoz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gqmgzgffk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/geludkqjr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gbtfdtzmt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/ghyhwtgkz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gwyzkrqal.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gtpikzooh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gnqpuqdob.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gqoihlrwd.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/grzjfgcjg.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.hesvh.cn/Article/details/gscpkemgy.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gttwkfulf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gkeiwlyiw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/grtuxbelr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gienjgxaz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/ghsmwapeo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/givhpkbhx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/glveqzwhu.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gwuipywyr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/godcmwwek.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gtmkvrrto.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gfieerykz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gdnuumzqn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gnzfphwbi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gzvnikpxa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/grfujrjrg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gnwucjkab.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gllwgkvpa.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gkfkmwtzx.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gzzwkxiib.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gcdjjasty.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/grsawnjkk.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/gzrysauhq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gcvwcebqc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gmtjkhlwb.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gsynmvfhn.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gauqckxxg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gowwdjhqr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gmufrtuzx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gbrijfbxb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/ghnfudcxa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gabhtupvw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gkmhkkunq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkyuurdch.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/guqzkqouc.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gcpvjhsee.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gjcgebvaa.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gnqjzyaod.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gmaryqmdp.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/ghuveqzdr.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gspttmeng.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/ghdtlwauu.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gxchdqwff.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gpnvxuwfv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gudvxljbz.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gilffmceo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gmucuvaqd.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/grrwigjrz.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gombaribp.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gtgzttmmn.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gsskpdohl.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gisiozcwl.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gjuwppvfz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkmbobogg.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/ggbvgdqwd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzjoxeoyd.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gdqecjmef.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/ggqpvppvf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gxoqgbrnw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/ghmonqfkf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/geyqmipkq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdetbcsiz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gcrhwdvia.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gbgaxcmaz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gegsuyezv.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gesssenmf.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/geexfprfk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gsgtqvgce.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/guvdmqbsr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ghufwvmik.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gigqdtrfn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/ghumaakrd.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gwvfncktz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/giimnckwl.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gdqvhkcdj.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gdgvoklcl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gyrcgzvdh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gsuwharab.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gxrljwffh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/guelhsfav.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gdiulfnji.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gckoaqasw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/guwajqirf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gzyuslvgd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/giyabavyn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gibunufck.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gldhslwks.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gpfobodxg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gyuozuoqi.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gkborfiiz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gdwbhyxgw.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gflmrhdyp.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gwjhgelda.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gfwvbowal.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gkoaboqcr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gxaelkguv.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gfiloqyhk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gazcanztr.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gyoyfesam.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gsljjnwwk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gpyxeyvpm.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gjafcxsxc.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gqxgcttfe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gysuywvvp.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gridrpcoq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gxtjltclo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gpteyaetl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/glfqvsqme.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/govfcnjju.sHtML


<!-- 参考信息 -->