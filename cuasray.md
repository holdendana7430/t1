代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://3g.zdbjq.cn/Article/details/gcxzhzcny.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.zdbjq.cn/Article/details/gdzzamkev.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gbpcabqui.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gdmtpodoc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gnvenatyr.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.fehbvm.com/Article/details/gxgkaxswc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.zdbjq.cn/Article/details/gjwprmlis.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.hesvh.cn/Article/details/gaeukmesq.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.hesvh.cn/Article/details/gjnupeljq.sHtML

[A19] 交换两个变量
来源：http://www.blog.zdbjq.cn/Article/details/godeunrwk.sHtML

Py:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/ggrzjamen.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.zdbjq.cn/Article/details/gupmskddz.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/gojwmghar.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/gouvqoqbf.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.hesvh.cn/Article/details/gndtsxbad.sHtML

Go:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/glvcyopeg.sHtML

Ruby: a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gzqahngrf.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.hesvh.cn/Article/details/gzpiwqwpg.sHtML

[A20] 读取标准输入
来源：http://read.share.fehbvm.com/Article/details/gmmvfqjmi.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/gekxfrkbk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.hesvh.cn/Article/details/gwodrbfxe.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/ggxgdjapn.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.hesvh.cn/Article/details/gvnowqaqw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/gkaqqianh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.zdbjq.cn/Article/details/gwgdkkhqz.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/gvhgrzxrd.sHtML

C#:   Console.ReadLine();
来源：http://blog.fehbvm.com/Article/details/gvpmhtyky.sHtML

[A21] 保留指定小数位输出
来源：http://blog.zdbjq.cn/Article/details/gjemladik.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.hesvh.cn/Article/details/gehyeyvzn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gmpumvrgj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxlyopjot.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gjlxaayat.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gyiqejkpe.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gaalpkrwq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/grhvxmmja.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.zdbjq.cn/Article/details/gmehlepgw.sHtML

[A22] 获取字符串长度
来源：http://wap.fehbvm.com/Article/details/gblavbick.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/guhtfxkit.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.zdbjq.cn/Article/details/gsgmmpved.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/gykxwszor.sHtML

TS:   s.length
来源：http://www.share.fehbvm.com/Article/details/ghonpbloq.sHtML

Java: s.length()
来源：http://baike.fehbvm.com/Article/details/gffnkwtcr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.zdbjq.cn/Article/details/gqkrbvmhh.sHtML

Ruby: s.length
来源：http://read.share.zdbjq.cn/Article/details/gceqivhdi.sHtML

C#:   s.Length
来源：http://wap.zdbjq.cn/Article/details/gtjutsntj.sHtML

[A23] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/grykspvkk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gelopxdwp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.hesvh.cn/Article/details/gmmmbrmqd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gngeenvwi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gtngwqgqi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gpoklibim.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.zdbjq.cn/Article/details/gsvfhupcy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gyetkztrm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gpavspoaf.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gtihjdmnu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/gnbythtwy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.zdbjq.cn/Article/details/gvdweadnk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gevcaqpwm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gaocykygy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.zdbjq.cn/Article/details/gjbmaynib.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/gxujlmoto.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.zdbjq.cn/Article/details/gvqfxphqa.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fehbvm.com/Article/details/geiyhqlrt.sHtML

[A25] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gcocyyhkg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/gdgebjdcb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.zdbjq.cn/Article/details/gnxdlunco.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/glaraemfr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/gyhnzkvhb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/gezbnuagj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gzyaszedn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fehbvm.com/Article/details/gvauflvjm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gyzmwergk.sHtML

[A26] 类型转换总览
来源：http://www.share.hesvh.cn/Article/details/glllrcyha.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.zdbjq.cn/Article/details/gbkvqeenr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gcqfefuby.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fehbvm.com/Article/details/gltfdcagl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.hesvh.cn/Article/details/gevbmobmh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gwqkaotel.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fehbvm.com/Article/details/gktetvxfu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.zdbjq.cn/Article/details/guvvyikys.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gzkqvskvg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbezupbnr.sHtML

B. 流程控制
来源：http://baike.fehbvm.com/Article/details/ghocjupby.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfibkxbtb.sHtML

[B01] 条件判断 if / else
来源：http://www.share.zdbjq.cn/Article/details/gohydzthi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/gnjxjdmze.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfxukifko.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/grfzwtdpm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gyyxvrwno.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gbnqikqyy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/ghnurlrid.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gdfbzsrlh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gputdttwv.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/gpblwuwff.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fehbvm.com/Article/details/gumomclzs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/gfiudwjco.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gixeqhpcy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/ghtehvgon.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gtevwuiwu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gwmnnvaez.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/gbvpyovyl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gnsrwkroe.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/gmsxnfeuw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/gdwllcgcr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gyozocmev.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gwgqkgexj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gkeeyhxfd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/godrkeapi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/gpuhivovr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gojiscapz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gknnvgqrx.sHtML

[B04] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gkrkmdyfd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfjbejv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fehbvm.com/Article/details/goknydlic.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gsmkognck.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/glkzhbcpa.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fehbvm.com/Article/details/gggoyorts.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gpyfyakla.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fehbvm.com/Article/details/ggnxwvnhv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gffevofwk.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gldgltmzg.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fehbvm.com/Article/details/geqonlcsp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/gigyautib.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/grocrdkdx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gvdoealzg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.hesvh.cn/Article/details/gkltanymk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/guastzyqb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/gnfidsoqu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fehbvm.com/Article/details/gtjmcpbnh.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/givvfgdfr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/ggsjjfrgx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/gsvhajfen.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gzhycicop.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gvvhlasbj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gmnjfldrh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.zdbjq.cn/Article/details/gezplwxxt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/gsamzwodb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcmzjvhas.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/geywelfle.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/gresbrivp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gkkgryjgt.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gualhbuvf.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ghfasdsnk.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gpfntsdul.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gbmmgvake.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gjtnvpqoo.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ghqoiqbba.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gosszsepm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/glrulurzp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gjkdaqviz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/ggzjgdndh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gdcvijphy.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/ghlacpkfp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/ggwzcscbj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/ggigtwnyv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gfbyorkji.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gpjnopvka.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gztydvyrs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gnrjbyyjm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gtovdhjwh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gbvupxass.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gngeznrza.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gsnppffhs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gjtsxwmbu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjujjqrq.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gwvveaffm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gmtkqalkt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjzfpnxds.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gzszcgjnb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/grtcockxv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/giezslkxy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gibwsvuok.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gmttvfgfi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gpxnsvpoj.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gkvddgsjp.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gljsypkrk.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/guahoewrq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gdfybimnd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gfyumuuwr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/grldzhyju.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gaxisrbfs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gipklgmdo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gkkmtxazc.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gwyjygzso.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/ggysgshpm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gotgwlbhd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gbtooiebk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/grmswwdqt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gxwiazavm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gvjdcbtgn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/ghzbyluvz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/giilvibdd.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/ggoiqomxq.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gnonoghjh.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gohewxkxy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gmsbgapnx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gvbtgehln.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gffrtesaj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gcisjsosb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gawzmwygm.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gebpstpdh.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/guzjgrslb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gzjjuxoai.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/grcsyjtfo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gangttboj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/griicvvii.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gscnmrmwf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gwqyvrhpm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpshnhspq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gdhacxefa.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gnjcfyyts.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gpprbtrdp.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/giwoeatlx.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gbxfcbzse.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gxsojfyop.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gclypmyan.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gwktrikek.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gccwyppxa.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gvsssskan.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/grmxfojoj.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gemqdhpsg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gsdiknpdt.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gbtrgbtdw.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gbyiekkgn.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/goatnfqvk.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/guitryitx.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/goxuahgvv.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gmhcdnqix.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwujxteqj.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gxdikexbo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbrudbnfw.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gqppwauvt.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gtskcmlzn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/guarsutau.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gdbwxessb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gguphefvh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gtgbmqlml.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/grmpfuxrw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/glubcyuff.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/giekrzynm.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gdmoonbmx.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gzwpjzuhu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gbyryhcov.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gagsqfnyj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gbbwqwjca.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gtxmhwlcf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gsbohvtpe.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gurcdqond.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gsxqcwaru.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/ghyqtuexr.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/ghrazxuqw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gomoqbscu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/ggaiptlqd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gfbdopvmn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/godmqjcfm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gglfxycvg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/goczletwv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gjmptdjvs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gpyhjtkaz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gimldclop.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/ggwrpzpik.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gctbihexw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gqxmqewuh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gddqmswho.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gsjkzhrlw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwdachpcm.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gyakscwke.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gcmhsjgqs.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gyquixkil.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gxvgwupdz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gpcwgviia.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gruxfnljo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gjublsfvt.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/goecxogqh.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gsaiohjkd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gjtxdulqi.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gpbenrxsl.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/ghyfwvekf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gwhmftoff.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gsdhqzqnn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gtsozvujv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gdwivfdaf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gpjwckzcn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/ghamiriht.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gxjvdduws.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gzlptorjm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gijeuautk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/grdabsywy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gnxwyhmik.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gqasejgqb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gmahpxeul.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gmjxlvfyu.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gxohyxorp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gqlslaaji.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gygdzsakx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gduvhozio.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/ganqshxxs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gvrmucdrv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gjzvqwopf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/ghufjpllp.sHtML


<!-- 参考信息 -->