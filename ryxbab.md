代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ayfqllhq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2znfhleyp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ovxfuufa.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hbuqmvrx.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gvuugeab.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2nyamzfnn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2xiffbasw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2rnbqzkvv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2gwyeecrv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2bmszpwvh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2yaxdsqft.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2vaxsoyxr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zixggcye.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2mnylkfbw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2hwqnklpc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2bdzsntbj.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2mzxvktyi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2owikjxrt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2iilejqij.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xxlnpioh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vwxnucny.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kwmuxxnj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2aifnczpr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ljmzbwxy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xsxzdrdh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqdzqeko.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2pidxeagd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2wsueuprz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mgpiadhd.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2uvncdvcm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2lkjkepdo.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2evxcgflo.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gmjasuje.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pwxagrzt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2gsirftqv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2udhxlqxa.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nmwetosi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lxqwwawy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2quleufmm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcqxnzhp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2indalqhp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2tfjfuokv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2vrdgtzdk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2grkjnodd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qwybiclj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ryruxopt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fbdlrmpp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2bxtcgizw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2nlkuqpow.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2kgrvewjf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2iivdxrde.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hpwpkvss.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2lpdxhdmr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2czpelzlu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2soppktwd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yfhtdogs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywjevkqe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wbyfvogp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2sckggldg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2sqwpqqnh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2kkmokkcl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2dfoqlfdd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2qiyfhzxk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2wkchmwqg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2xibjpxyu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kmcnrpck.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2pvjmsyqd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2gltwivcr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ponvcziz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjiywliq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ctltmeor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vyokhzyo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2cnqgnibz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jbwbjdjl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aipqhvll.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vyigovju.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dpbtsgao.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yolxjpps.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2gzvssgry.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2fuenzbes.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2eivtfkew.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2mjxrnvan.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xdbcmyrj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ypyfrcsm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mkcmbdcy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nwjvpvel.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2phsdrrle.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2vkykunru.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2oypxdjfg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qnojdilw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gyqtbtoo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ydsfocya.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2opsfadqa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2owvzdkyy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gucbompl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aauynzmp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2njraimdb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2dzqwqbtg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ppuxvdtw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ofkjhbfo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2mzxfpzxs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdnxunpb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ajgupqqk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2eiojvitl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bczcvyzt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2cmcifpyp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2rmjrjzep.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2lcnklfrp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2utbcdyxz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2cczeplfr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vixhgvhp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwhjchzt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pvxrddgd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvdxgcrb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fwhgjaid.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ajllbfag.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dsvhjvuh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2fcdldobl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qqohzydt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfirukku.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ouluntzh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpnfjotw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2aijeayco.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2otciiftq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2gkodfzfx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzbdkkob.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2szmolbim.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2dvfvaosy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccqcpwlx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sjtsfsqj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hglwbfrk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjefqcbx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wwkvazln.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ewkjkxix.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jeyoiacl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2lfknvjcn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2acwdhlqz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qfpgeisz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bblexmll.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2udgvuxda.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rgbxizsc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cswofkna.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2sgzxbuuv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2anturmop.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2afsidcob.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2rpmdpwkj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzgilnjh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpoddpwj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fzrfknia.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oinssplq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lcdrohwi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ejspurcc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ouftyqzt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2vtvplpfa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2nilqhxlu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2mvsinanp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2uuekfvzt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wriohowg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2hasmagcx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2nimdlbie.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ouijxith.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pobktjoc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xluchppe.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2tyxexybs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2sxlpgfmb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2srbusiuz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dzkwqcus.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pefistnt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2qzeblmew.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zofzyotf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mffeekhz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2whrajusv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ozyxhiwb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2dvcgewwj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2knhspeks.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vwkufnhg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yuucedsx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vbodyhdt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qucalufv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2aysarjpm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rxkqylno.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2eyoefbjy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2binhrlss.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2arspnnzz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mrhitcyq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2dbxdafxs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wqutumek.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2rpuojkzr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2cqwwycyo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2fzsuidtk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2hppodjlk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2cnqsylkw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwvmakku.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2savhgiai.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2utaojnyn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2voipeabk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hjqxwdne.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xgifsepd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2cdnnyetj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gjluybsx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2anftwjzt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mcopmhpp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fcgmramw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2npjjmjgq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gqvjlelt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mtlmimyi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ukdgsvxf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qronynma.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ozggufhc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpvjmwgy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lbukayvx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hmcdbcvc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2odaafjem.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2eirprrvk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2lojjeaxr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zwfclefy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyvnhsly.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2llmberev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odhkvfwa.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2auteoryq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wiyyqixg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bcppakwe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ljqpbnmy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gdiyntxa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqqeasvx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2yyraklnq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wcisigoz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gqfzkaxw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yjbnlefs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ebwzohfs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wehskhxi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpfqgxhh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fcrwzmks.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2umkllsgg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2repdcttw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2gkoppfsc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2cpeymbsm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2iroeuvee.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hclqabaz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2roocrypm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtkwblqr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sbjvrwmc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxxqikgk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2vcqeciql.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xamklfdh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2subukujv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lcmeotfx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2rlnwvajr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hmpxamgl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxqzjxho.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2loizgfqk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2inxmzypr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ahlvwpvn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pmlmkwia.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2axkbuwby.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2brhmmxxx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2eyqefxzx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ciyogpxl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2avktdown.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vbxtaysg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2honxizfn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2epndxqrw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2jrimnekw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2tawjxvtp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zssqumhv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ouoasili.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2zszqcgig.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vklovdpe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iskguxbo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kglgvomt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vpnwzhhv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ygjsjied.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2btzadgtb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2jjjvzott.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2kdhvdebi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2shprvctq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2lmfntrkw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xniuwuwg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dqffvrbs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2mdbqdmge.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2pebfzdgw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ylmyxftf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2igafcbzv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2jmmyzzbc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xasndkfb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxudstll.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iemchprs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2fsoobmna.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2qiwmtils.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2bsqwrffp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlllogob.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2gussbufj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxfhtxse.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hhwibaeo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yowxgjye.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2algibiyl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofvisynw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lcrhsjpu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkagktkb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ioaknxfh.html


<!-- 参考信息 -->