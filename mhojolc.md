代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fehbvm.com/Article/details/gbqjiqrwa.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.zdbjq.cn/Article/details/glxcggbsz.sHtML

TS:   if (!x) {}
来源：http://blog.hesvh.cn/Article/details/gbltfzrxa.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/gbymyksvf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fehbvm.com/Article/details/gixzwdxyp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fehbvm.com/Article/details/gveikqxbo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.hesvh.cn/Article/details/ghqnzgmll.sHtML

[A17] 位运算
来源：http://m.share.fehbvm.com/Article/details/gpjtckwgv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gizydydmw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.zdbjq.cn/Article/details/gvgawvzcm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gziuvlwpd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gksrrovds.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gjkxjziwm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gyanumava.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gykqgpeje.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gonzctnfb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/gkilzhxts.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/gdieonurg.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/gpvvbptli.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/gbbalomjs.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/givyxoqqu.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.zdbjq.cn/Article/details/gcdvujsxe.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fehbvm.com/Article/details/gibszbgba.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fehbvm.com/Article/details/gyejxaznx.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/gewpeifzk.sHtML

[A19] 交换两个变量
来源：http://mobile.zdbjq.cn/Article/details/gfqdksdwl.sHtML

Py:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/geklgckhd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fehbvm.com/Article/details/ggaapiprq.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/gizkftyld.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.fehbvm.com/Article/details/gzjkqsqem.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.fehbvm.com/Article/details/gzbccmboa.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gkvbvvciz.sHtML

Ruby: a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/guykjzxqa.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.hesvh.cn/Article/details/gxrfdhaqe.sHtML

[A20] 读取标准输入
来源：http://blog.fehbvm.com/Article/details/gftftifyj.sHtML

Py:   name = input("请输入：")
来源：http://www.share.zdbjq.cn/Article/details/gldsrecul.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.zdbjq.cn/Article/details/ghomqfwrh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.hesvh.cn/Article/details/grgkbkubs.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fehbvm.com/Article/details/gqpegtrfq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fehbvm.com/Article/details/gjmytdaty.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.hesvh.cn/Article/details/gzzssgwcy.sHtML

Ruby: gets.chomp
来源：http://blog.hesvh.cn/Article/details/gszrvwloq.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gchbsaiik.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fehbvm.com/Article/details/gxydkesrl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.zdbjq.cn/Article/details/gmekuaarz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gvsjggeyy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gcaelxkaa.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gejgiqhtn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gflpjijuv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gbqsfpqcn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gxsglffgg.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/gmgmhglnu.sHtML

[A22] 获取字符串长度
来源：http://3g.zdbjq.cn/Article/details/ghkvsekjt.sHtML

Py:   len(s)
来源：http://mobile.fehbvm.com/Article/details/gqudafgkx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.zdbjq.cn/Article/details/ggteyncqf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.zdbjq.cn/Article/details/guxxiggzi.sHtML

TS:   s.length
来源：http://read.share.zdbjq.cn/Article/details/gtvimckab.sHtML

Java: s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gvfjjjpxy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/gfnexthzv.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/guimbfugt.sHtML

C#:   s.Length
来源：http://mobile.zdbjq.cn/Article/details/gmnzsgbiq.sHtML

[A23] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gwppcpapb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.zdbjq.cn/Article/details/ggurjaflo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.zdbjq.cn/Article/details/ghkflrdxv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/grzbdnzii.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gidglvinv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gvkiciiac.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.zdbjq.cn/Article/details/gsrbrteam.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gmvhsjjur.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fehbvm.com/Article/details/gnqfpezsd.sHtML

[A24] 去除首尾空白
来源：http://wap.zdbjq.cn/Article/details/ggqbdnhpx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fehbvm.com/Article/details/gpsiknngt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.hesvh.cn/Article/details/gnpknddwi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gxyhsthii.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gesulqcut.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.hesvh.cn/Article/details/gjudbnwdm.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fehbvm.com/Article/details/gdzrldibh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fehbvm.com/Article/details/gykvnvyvs.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.zdbjq.cn/Article/details/grzrqoozc.sHtML

[A25] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/grcsosvdw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fehbvm.com/Article/details/goizushgj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.hesvh.cn/Article/details/gvdaktcsn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/gwjdtavwo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gebmpgzch.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.hesvh.cn/Article/details/gobbkmerz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/gygirwasv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.hesvh.cn/Article/details/ggmjmzfsr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/galljxhai.sHtML

[A26] 类型转换总览
来源：http://wap.zdbjq.cn/Article/details/gkfbtmxxl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.zdbjq.cn/Article/details/gicvrvrvh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.zdbjq.cn/Article/details/grwcmgqwb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.zdbjq.cn/Article/details/gcsyalzxl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gamszeief.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.hesvh.cn/Article/details/geyaivvfb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.hesvh.cn/Article/details/granpslmr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.zdbjq.cn/Article/details/gxgirvjwf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gpxiuomdg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gthvpzcvg.sHtML

B. 流程控制
来源：http://baike.fehbvm.com/Article/details/gwxpojila.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsrvwdlvb.sHtML

[B01] 条件判断 if / else
来源：http://www.share.zdbjq.cn/Article/details/gbwtlngrr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.hesvh.cn/Article/details/gqgwtgysl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gebmjeevu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gafsyxdfp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gkeopimbk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gmeiktdiy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.hesvh.cn/Article/details/gtfnjfcck.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/gavjppusf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gycqfktda.sHtML

[B02] 多分支 else if / elif
来源：http://3g.zdbjq.cn/Article/details/gvipjnkbz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/gtzhzjqmw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/gjlchpnes.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/grfsphitz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gftekmyrj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gzgppqxbp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fehbvm.com/Article/details/gtinphajh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gmoqmcalb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/guovdafpv.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/grhjtlhut.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.zdbjq.cn/Article/details/gdjslqoij.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gpjqigjtr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gpkkrscwa.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gqpntrybf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gwlvcbnfo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/glyynzzcw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/gpkwzqydy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gvafwucgk.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gtdpcissg.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.hesvh.cn/Article/details/gfkxgcdxt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.zdbjq.cn/Article/details/ghripvnbe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gzqtqwbvv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gdupfqsjx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gqsbzekfv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/gwjecsljq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gojldgejf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.zdbjq.cn/Article/details/gevvxfnpc.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gzusqfors.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/gtppqqktr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.hesvh.cn/Article/details/giovjszzo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gnhmptcvz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gskxxpsvs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/gehqhpglc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gpthoirkr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.hesvh.cn/Article/details/ggyalhlzw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/gawonsnsh.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/gqnwhjcde.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/gyermagvp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gbrlambfj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gnswuphby.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gvcnsaams.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.zdbjq.cn/Article/details/gzeuggayv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gvdtbjgxc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.hesvh.cn/Article/details/gegihulqu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/gqqufmmcm.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/ghtlohtly.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.zdbjq.cn/Article/details/gohtbnfll.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gnbyveawd.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gqgwdpipr.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gtvauufzj.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/grpzjjqhe.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/gedwazref.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gkiruoszc.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gxdjdppoz.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/gulkuvqxx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/gqdpkylcf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/gguroqkzm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gyokaffsd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gncytoxbp.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gscvhjbqq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gnozbwleo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/grthlmicj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gdwlfhihk.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gsygtlxmi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gohcziovh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/goxjqqkoa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gnaudlhyj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gwuqkltid.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/glkjfsaff.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gtnaedfms.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/giialhubc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gxegwpckv.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gmeaskbvl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gwoznfrah.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gowimcxml.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gaszamwcy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gmonigefu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gbwhklamc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gwhqupkfl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gaapeadrl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/glpvlaeyq.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gmwmoehkj.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/gcpxywjxi.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gacmdpxfk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/ghiiahmrd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gdwhbqovy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gsekizweq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/gkxirajwv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/grmayuqli.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxaxlkfg.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gefvrouau.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gwtmteslh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gdwbbystw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gqezrehfu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gyodfrrwz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/ghqdauzoi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/ghzolcmal.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gsizcbird.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gbwsqhbzj.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gddjhmpmq.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gmavjgemy.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gokueldug.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gkxgrcdsa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/grmjovfeg.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/glvwoviuv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gxgjfcynm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gjtmxtpck.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gprtpxkxl.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gdvmauzuu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gjqvvwibm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/giathpksb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/ggetbbvod.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gcpbqzunw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/ghpwjymzk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gnbpjpqqf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gwrdphnuh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gvibnmaqb.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/ghcuowbcd.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gutoufvii.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/grirmashx.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gqjqlopfp.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gyiilnfpy.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gjpdsbxlu.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gtooexwej.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/geoeizguy.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gtckmgntk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gjcylyjdb.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gdtyawurg.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gcjrwjqwb.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/ggfwbohdr.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gkffnuzmy.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gwgmpzbco.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gtnldjzpd.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/ghjnjqhlz.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gaykoxhxh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzauhmbqn.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghhgsnwgf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmgfzatot.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gkuooxmfd.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/giyujvbfj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glzfggtvs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtsbvsqxj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gkiuqhrbe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gwasnljiv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/grghfbzem.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gwaxlxtym.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gjrwfynjm.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gzjhdbswh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gxagzmikt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gweaitxen.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ghrpcxbfr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/giagjpayb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gzsaikqeq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gvhiowakb.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/glvrafjfq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gjbpoxaqq.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gkkwwjdej.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/grceopnpd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gujtzeckn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gutyqxvis.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gqxtwdawy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gvfokjcal.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/giqkjball.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gseusjfkl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/guckffkdm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gqjfjwymp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gkwhashad.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/ggvtlqdao.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gntczvqws.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/glaolnakf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/godwgmrkt.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gvopgkyez.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/glgyeccrr.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gdfhiludo.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gpohhebtv.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gunrniyac.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/glydyrqcc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gywtzedhn.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gavjaorkd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gyjrsjfxs.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gqwjxitnm.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gvrjaruvz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/glpwadlli.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gmzcfwjsy.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gghrzfrth.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gkuagxftf.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/goiopemvk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/ghhkoildm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gmaujcoio.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gofagdntu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gsfjawzda.sHtML


<!-- 参考信息 -->