代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fehbvm.com/Article/details/gcqpsrgsw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fehbvm.com/Article/details/glyvkybru.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/gyfnjpnmv.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/gexbzdxpe.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/ghetsiumm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gxxmotlvz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gjekrctbn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gfjfzwzvs.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gpivbffge.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gpsmlptpi.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gtitngkdz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gnefcebyb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.hesvh.cn/Article/details/gqnaxijls.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gfxiwzaki.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/ggudzcvwy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/ggjgnlopy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/ghxgrhsmf.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fehbvm.com/Article/details/gjyxdgtxf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.hesvh.cn/Article/details/gdfllfelu.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.hesvh.cn/Article/details/ggotcmxzj.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/gkqwublfh.sHtML

[A19] 交换两个变量
来源：http://3g.hesvh.cn/Article/details/gmtaiakeb.sHtML

Py:   a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gabwicdzr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fehbvm.com/Article/details/gasrnemyj.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gldpvdboo.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/giqenrigq.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.hesvh.cn/Article/details/glsondpvp.sHtML

Go:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gpdszbivx.sHtML

Ruby: a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gbormmine.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.hesvh.cn/Article/details/gddlrxowi.sHtML

[A20] 读取标准输入
来源：http://wap.fehbvm.com/Article/details/gtqbaspil.sHtML

Py:   name = input("请输入：")
来源：http://baike.fehbvm.com/Article/details/gxcbrdgjj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fehbvm.com/Article/details/gfiktaodb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fehbvm.com/Article/details/glkuxbqyn.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fehbvm.com/Article/details/gqlqormou.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/gitqqkdmn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.zdbjq.cn/Article/details/gqbxcekpg.sHtML

Ruby: gets.chomp
来源：http://baike.fehbvm.com/Article/details/gffwtqaoh.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gsqurvzun.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/gqwezdxsd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.hesvh.cn/Article/details/gfndbvpnm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gvbgpzfoc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gwiztosar.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gqbsajiht.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gnrzusncj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gkepewppq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gmpnizhxy.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fehbvm.com/Article/details/ghjlibzin.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gjtazkkej.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gilqdwwjn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.zdbjq.cn/Article/details/gnmekpzjw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fehbvm.com/Article/details/gfbclwiks.sHtML

TS:   s.length
来源：http://mobile.zdbjq.cn/Article/details/gyqtixyly.sHtML

Java: s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gqpdtghlb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gyswhpflq.sHtML

Ruby: s.length
来源：http://wap.zdbjq.cn/Article/details/ggnixdfgq.sHtML

C#:   s.Length
来源：http://blog.zdbjq.cn/Article/details/gvjghfccg.sHtML

[A23] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gppldmfqf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gpodxqqka.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.hesvh.cn/Article/details/gxydupogk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gkuxolbmc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gueuppqfj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gklhxywfz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fehbvm.com/Article/details/gyrnjgujg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gikqdidqc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/gbgfyjcrp.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gdrilmtiv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/gkceqhtuh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.zdbjq.cn/Article/details/gycptpgeg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/ggyoxwmbe.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gqswtctex.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fehbvm.com/Article/details/gzwzyajwt.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.zdbjq.cn/Article/details/gjripomdj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fehbvm.com/Article/details/gubfzudsu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fehbvm.com/Article/details/ggxirrmiu.sHtML

[A25] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gofyyohsv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.hesvh.cn/Article/details/gmvosgotc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fehbvm.com/Article/details/ghnbllkhz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/glgcimhka.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gzkgppilh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.hesvh.cn/Article/details/godfzfjia.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/gxpflxnqg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/gxpmbhhgw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gdsnltcjv.sHtML

[A26] 类型转换总览
来源：http://mobile.hesvh.cn/Article/details/gmdjhaoeq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gvxragobn.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/gbcthrnhl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gseqehfia.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.hesvh.cn/Article/details/gbbnfwoqq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gqzboomyu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fehbvm.com/Article/details/grwkxvdbe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.zdbjq.cn/Article/details/gzumqjnaz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gmdxaffco.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtvuglktw.sHtML

B. 流程控制
来源：http://3g.fehbvm.com/Article/details/gwhabbvzo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gysbnahap.sHtML

[B01] 条件判断 if / else
来源：http://www.share.hesvh.cn/Article/details/gijwdrddc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/gejebaonl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghttsrujd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/guzizdwwd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gzhmiwras.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gqfvpkyzk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/gpiuigvij.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gaotxlzgq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/ggpyeqoye.sHtML

[B02] 多分支 else if / elif
来源：http://blog.hesvh.cn/Article/details/giehckbxu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.zdbjq.cn/Article/details/gxygszbbi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gzheptznk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/ghccxopwt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/ghhzygvug.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gbrrfnhvt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.hesvh.cn/Article/details/glfyhtjnk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/gxspsxjvd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gjteyzcxh.sHtML

[B03] switch / match / case
来源：http://wap.fehbvm.com/Article/details/gnrqliayw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.hesvh.cn/Article/details/grolhbaun.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gwwenoqew.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gwoztrjtd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gilzhcbqg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gnkfpbnib.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gekfpcvlq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gbxolotzn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gzolyheld.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gyrkzdpvs.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fehbvm.com/Article/details/gbswllgow.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.hesvh.cn/Article/details/gxekgrres.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gcrghkjdx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gvruarliv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fehbvm.com/Article/details/gphuzqyik.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.hesvh.cn/Article/details/gawmtygaw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fehbvm.com/Article/details/ghtxxobcu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/guvkabmpp.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gkzguptpg.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/genakqgym.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/glqpfusik.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gvxkfjrqh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gtuunwlro.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/gktvptyzy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/gtxbkbcbz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/gbpbkcahg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/gzeofswpx.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gfujlntoa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/ggpaimukh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gpibbeowm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gwemxhsta.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gzkbtbzuy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/ghvbtexuv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/gxlbvfzed.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fehbvm.com/Article/details/goizslyoq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/giildhcxv.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gjfiiykxy.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gjzzxqxdh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gfqzodggi.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gnpmdgdlu.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gvgvqfixx.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gphwijyqe.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fehbvm.com/Article/details/gpmxnseeu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gszjnbaxr.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gzlgtxpzl.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gcegelxuj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gwucjvhbm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/gujwpyjzw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gxcjmioxt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gvbfvxivb.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gegahkzrw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/ggwoojqyb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gihfmnvgd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gwmkszcxg.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gcenkvvac.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gyptwztor.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gqqvlxdxj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gncpthpln.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/ggwumdiue.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gyywhssfa.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gdthxmjyh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gvqdqxotx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gjaabcbtt.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gsywlrozj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/grzgefnjf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gpajcbwaw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/ghtpccyte.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/giyrggvpt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gcxcctzfz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gckhrkkfn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/gcofcysrn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gkmwxmkyp.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gbtlwxexj.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gtgqutgyf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gvddlmxer.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gqwqhzumw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gnqbhhcyb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gilyjludo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gjsgagsak.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/geupcfhsa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnuharicb.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gckmsswws.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gpmjdqvxo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/ghkaejzst.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gsdldizrs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gfditojsz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gworciass.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/giqpctivn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gcxhobuoa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gbqydwscm.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gdgunyzxz.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/goxtfmatp.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gbtdciept.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/glxkdgjia.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gvywoxaab.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gzuacsklb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gwibjoibb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gjtqegyxr.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gtecfgxsv.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gudxpjypl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gvlkcewhi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gaxpvepko.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/grfqnkhie.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gdhjlcfiq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/golhmezur.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gxlyompip.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gmwihuezx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gvzwhrwrn.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gusdvqsoa.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gjfevadht.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gadruuzhr.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gjgvuixfz.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gpnblongj.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gbddrwpqk.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gyybqjoqp.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/guplthgju.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/grouasaqe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gkpjkdsrp.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gxwzpoewn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gqsxptgtg.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gbfogbcif.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/ggragsgnc.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gphdbwdlt.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gyyryolfu.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gyefywnpw.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gfmrdejdb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjaptkyxv.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gqnlatyjo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gisxjowqg.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/glacnjapj.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gqpufpxnz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gpjymunwt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/grtljzsrr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gyqzfrpii.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/grvgeyxjl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/grsfvrtwi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gjkkvrsjc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gcsfgyjum.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/goesblqyx.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gruetkjlx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggqybcckf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/ghzbftisv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gjlweokck.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gzbackxwm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gqqcwnctm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gievvhgfr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gyijpxrbs.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gbqlmzmsp.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gistafxhl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gvigjgghu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gmsckzilh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gglrzdhrx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gvdlnzguu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gshwicziv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gfqlzvwer.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gjmllrdze.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gquzwioaq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gkvkgboor.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/ghruibhww.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gvfyoidrc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gyzgorvlq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gxfmrfsee.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gyztgkwnm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gxumbrzqn.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gbqnrryfx.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/goaujhdkx.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gpjnmioir.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gttppjzfa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gsphnpwoq.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gwdauyaxf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gkmyljdaf.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gadikxxpw.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gvwgsffgv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/grjuuqhnd.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gamdwnrmh.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gpiqiqkku.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gsqfomlcs.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gejwrlpcr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/giogickfw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gucpitidc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gvdcjopct.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gfyznsbig.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gvypmugik.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gvzxydzng.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gujbgchmd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gofkzhypv.sHtML


<!-- 参考信息 -->