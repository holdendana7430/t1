代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2scyihevx.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2pxhaestr.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kttjnvfy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2sedkshym.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2jfzrykqn.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2oyzcamcy.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2fyahlbot.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2pkenxqrh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ryidcaci.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2qgvbihoc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2udcaguzy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2wsnctrrh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2xrnferps.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2mfnivmoc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2jdzcfavz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2mzuioatq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2dzyhfkaz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ifarizwg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2vmadwbym.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2hqvdggzo.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2gdhudifl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2llvwtrfl.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ftmsvyyq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qyuzgnyf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bxemovtk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hsagpwzn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dwtmkjth.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2btwfccdz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2prrfynqu.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ppnblcet.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2nqzjvtmh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2uprbzmru.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nomyanrk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lxxnlznn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ptlcoxvl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2aluzxzji.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wltcfvwe.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xdaqiwpc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nbjzezkn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vulrvufz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ktqkwpop.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ztijtofu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dbahlgnw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2wslsldkr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ygtookmc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2sccpjnpt.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2jrchhbvv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2sbmhmwfg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rexgxsoh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2stziuquk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ufasacxf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2cjnwbvtz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lsexnwwi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2nqigwtjg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zxlvfkio.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nanoihhl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ikyfarss.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jsdumqwy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2harzhwin.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2uuhdaved.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2oqypoewf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pxgdeijk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2tyujqkoj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mcucuatq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ytcrgypq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2vzxibavs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2onbliewc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2nyakhrwu.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2flyvvitx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ghgoxrln.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2lqiaflur.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ltesklxx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jskgcctg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hioapgtn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2mqiynwaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqckijzm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xyixwkzw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2owtidukx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvezivdj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ojdyvccw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2eadhwajy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2etsgyjuc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2zlcangho.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2myowtrks.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rkpjuaor.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2worxrxbp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2qavzhkik.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qexnwumv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cgfozraq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2myvmrfsk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uedvtokm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jzoswdwz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lnvooiiq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qzvrfojy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2uhhdokpx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2pwyzjyhs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gqyrwmef.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2drwwgeav.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hzchrbdh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kplaciqy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2najewfln.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2cnopgvhh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2srgqdwcb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cvkdkzbe.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2bzcripzs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2srsxjzph.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2noiuowlx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bctyacko.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ewwowbqk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2sxmtonzv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2jzxetfxu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxakvsww.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dpneegan.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wmqdzoab.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2eyfdlhto.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ojagrell.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwdrdyfy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdaruqsk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2trkserua.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2fewsbzbq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xzlhqdyt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2wrinhsfj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xeghwvha.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qtfzvjjt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gckhzlsd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lpjssedo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jwifebsj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2plyeqvgc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qbefvcid.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2qfhiebpr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2sntkvuzw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2azxdfzsl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2acvvszkt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2foesalqw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zzilfzaj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zehllbbk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2dxhlfwzu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2mzjcpioj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tjouomoa.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ojabwyer.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2pzjdcbxs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2unsuwgkw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gfvtbxyk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tqxpibrx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ruymedhd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gyxdatom.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2fnzrbcwz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wjehiaql.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ixkvylpk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vnhjtjwv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ihmcrvdw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jwrucunf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pazkaair.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzkwalwz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zhtdexlv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hescampw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yqmlmohg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rjmyvdup.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ipudulpl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2yxjbnuqh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bbejhunv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cucceodq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2yntnnldv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2iaqwrpzf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fdbdnyuh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ndclzboe.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2mnruwzmo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2dzhyjygh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uxzydubi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wgbfogag.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bpwtkvqc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tsfprgde.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gbtmiyla.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2domfkyha.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qtipuqcl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2salkwter.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2eracwneo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ppbhorfj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cqmuulhh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nlvrizni.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2augblpwh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2yzsryckh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2txlxtwql.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2qripdhhv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2icmphobw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2fnxvxvby.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfxndims.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvtooojj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2omsuvybt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2syyuzmcg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2avpgjymo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2oyyuzxfv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qqwrhhrf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xaykplvo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2cdqgastz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ckxchgok.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfncselw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wxennkcm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ptmzgahi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dswnhwbn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ltezahan.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vfvlrtqt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qfhcasyb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2lhqdpnvm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2bzpfbqts.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2igdhwkim.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kptebqzv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cypwukkr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hlkudqdv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2frjtidyw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zoowifpu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2dnejuarb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vcbepyhl.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2knkuhvqj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2txlljhpb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bmsoqkgp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2eqjxhwpp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jyqvqxxz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2fhcgeaos.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ctblhvdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eooiixym.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2idvzcdkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fenvllkt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wmswrpfe.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2buougepr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ynklmnyr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruzsidvb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dweqcziw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nurjkkrv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gljyzfnx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2hmvodrdu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nvqjyege.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2lrkkdtem.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2kovovzsm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ohtszlux.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ecrpxuoy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ayyzrono.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2eceavvsm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vynfcjoe.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hjfmzkbg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jkctjlin.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2lbxsnuda.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bapfhrrp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wecinari.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmgejbye.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjgbwftm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yiwrwffs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2spjqmpmn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2dadhyerm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2whxyevhr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kqewywws.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2esntvxln.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qupwltfq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvonhrfg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lkytfyus.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2uoulrzih.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jciwrebh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cenvvryf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gzcucfvn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2oilnjnii.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2taeexxwp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2seydfbzh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gavgbbrg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xafqslhh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2sagzxwwn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2batluyzp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jetaymwk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2balicpzv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2rigztbbt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2fruwszdy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hsnbnkvf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qpzpplof.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gxflruup.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xsqqwyrz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hoothior.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sntpngwx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uojoqtyz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bhwwwipa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2pmbectnu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bvtmakbx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2scskdszq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2jikcptra.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2vztoeoct.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2isewxayp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2atmxcebt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2izlfsoft.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gpmhoste.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gtgxgjqz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbmugwbr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iiwsrawx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xmgyyylx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dbimuilh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ornwzcbg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2awnsrcap.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxcpiqjv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jfatydxh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nksgizeb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgbpvxrt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yzdixrno.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2eujmblnz.html


<!-- 参考信息 -->