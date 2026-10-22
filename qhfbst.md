代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2iyofsyvf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ckdaabrh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2rbqsfhfs.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ugdhrtll.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2avlnsqyh.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2fwgvfgyh.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yumpcrpc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2iwhuylmj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2onagyiuc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2izyliyos.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2iylrkjoy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2iegpkmzg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jwqiukkr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2hhacqmui.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2gdhokvfk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2wpawdkte.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ksjvocgu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ckjmzqsk.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sixhyyps.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2qzoozohe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ugsywwux.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2axbsxxyy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2wcotzlon.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2xnfislqb.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2zbhejmfc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tyarkcna.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cdgkdnfe.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrkblklg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fivqygvg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vmotnqdl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yftorjop.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2yqexfsyb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jdiwssqk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2rtbbzmho.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qtzthjlx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wnomzxri.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sjormgzr.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mmvaahsw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2tjleuqgx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2mgvaosmn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2djqgnnmv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2olbmjgix.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2necahlpp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zkzekpkl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jejskgal.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uzcnoyvm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2egfzazgv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2cksgsilt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ucymymse.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2btsjinnm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2mutrdxfd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2qhlkixyp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nvzbiitd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lsiklyib.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hoszdwfj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ibxtwpya.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ptczxiai.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2mdormsnl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ksowiedv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vsuduvvu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2igwbrjaa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxvjpuyd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eenhemxf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nuecacnv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jcmyfkem.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ovsrqsyj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ntnnwcgj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rxrqspdo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2gashgcsc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2lvyslxzn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2vuyovqdd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2vupptclm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2urvxwysa.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vxnimnmb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2kidytcxg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2sxpvdezv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hehnhokk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ospgufpe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2xdlcebte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skhzdolc.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2dwpsvebr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2czfnfpec.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2fkqeevyv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gncytxba.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ytjgxsdv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qvlypntu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2vzghevpq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tkqhzqun.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gxokelak.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2zalnsjgu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2rspfyajw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrtvueox.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bmzqevvl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2orcgebot.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kroyeobc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2pumhuaye.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2szxjgyek.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2slefabdi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ovtikgsn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xwtyrwgo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hwysmvft.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2czuzlsdz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggmkgigs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rcsofrni.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2syeqxang.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2pafkkexe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2qapogckt.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bpyuqdgh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zgldfncc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2llefsibz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecxcwyro.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwrperll.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjtgxaoc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2sczxeqnq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2oqughaix.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjnuspbx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cvpqtque.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xjeifjgx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2mdxqznvq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2igjunlay.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2slefwbkg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2jpvoqkix.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2cgseaesp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2tuibwwgt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zizljdja.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2hmwcfiwc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qifycxaf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrimfbtg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2goemudzg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxsyshcc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jhlufiav.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2vymufrjo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2wcyrmebo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2wwznkahu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bjwnmkct.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ljsnptur.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2asdkeghr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ttlnjioe.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2toaehvyx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cckmhizf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hqzbqibm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2npwbrium.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2olvvnwyi.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2azncreaj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2lgpnvxtg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2craoqwnl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mndfkheh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kjhyhkjt.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yiprksly.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ckjwbvhp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2mnccoluq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2huhnyfdv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2fmxnrmhz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2nngzrdkg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2evppxgyb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfmlhqob.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyplupgj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpjzgkbq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2eojkxxey.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2cqadmawn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xwuoskri.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ambhoncz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ttepurum.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezqumtuq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ltqhfjrp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ghrvddlp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ecgvmstu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2sgufythz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2oxelkkfm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dklfakxn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ulcxftcu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2opyrdrkw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2akxyulcd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uaqyiqmk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2phwcngci.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ijwombyf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2pumaidgt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2pxgmfhqp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2scgjjhkn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xmvzmaco.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fgtopadc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vduuoyux.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yrbfipyg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mtmhacpx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2csajugdz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ekvhmkma.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rtuxexex.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2tedqkuxl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2lpspmlxx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qgibkuvr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wzciqdlm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2abtlautx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2umlnxapj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vurtqlgk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2mvtkfzut.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ffqkdisz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xdikwskx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2eqdjtxuk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2yvgrukty.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sgxmmmfj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2njfkiadz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zaakaqys.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mnaiiyhh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ubeccini.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bymbimod.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxazliml.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2hxzssvjv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2dsgbkgvq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ghstjnam.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vcuhhtll.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hqfxvxvn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hbiyauia.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gydizlkf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rmirvgni.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qaynwnav.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2zzalmios.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2rpmmfaay.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2pkiqzxpm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bebbrdjv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2afvxknfk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hvqzellw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ocpetfkz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2hvnfsagv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ndtfuuss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnpbyeht.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2szjvzdsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxxgsmov.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ogxairef.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mzoauoib.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2axhulzte.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2llsoodfb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydgfqgzc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyeupasn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zcxeekzu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2nqktvmvh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gxjpgejz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2iecnegex.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2rmunwanf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqpoliyl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hsreckba.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cebuscdw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2orrhgfjp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2duqwvlyr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vfbyqmpn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2oihxrayl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2brzclkfn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2pjbrswia.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2sornvlwa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2oiowccei.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qtfyguvl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvdkfnri.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ssztwlxz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2bdbmamkh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2lpexeolk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2yxrpczht.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2qivagatv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2onqmnxtn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2evzfkanv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2taxrnvql.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xzluzewl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2mqftyesh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tgjsppyn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gtnblzgg.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2nfnygesv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2aczyasxi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ajlgppsy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2chnqhdss.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rguuwqba.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2qerxdhtj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2iwwegrom.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2vwqsegws.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2tfqcwwvp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ppbjyyrl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2hsmyexyl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vztweipc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pcgmxlul.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cjfaoiwi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uinbzocq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wxwkuqji.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2igtewbxu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jkoqefoy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2oirxwcrd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2yzblayrj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wixpibov.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2dsbqcgqc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2bmukdlmh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eexmxjto.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bzsdtdpa.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2gdtelmmy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2tjdamyjt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jzbviczf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fqiobhom.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgryjavq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mcafbnbs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpkwktgq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rbaxjukc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2csydpyeg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2fxeqaowt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zkjpcypl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2hodkjcdn.html


<!-- 参考信息 -->