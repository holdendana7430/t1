代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ltkdwrxv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2gylatwtp.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2cuuxugtf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2kezjqxax.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2reszktda.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2zmsqkkvy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2gdhojbtb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ujsxmtss.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2yfhpnqqo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vihajdso.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2lbhopgpn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vzbqofqn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2aoziddpq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bmixrdbc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2saujwcjj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2rjslfrjn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kryfugnz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2wrrdbquy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2wghgtelt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2xzcaazbb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tagngghd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eydxyeyy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2vkdypfqb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2qfdzqpjh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tpjbpkoy.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yruttxpb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mwgqqvnb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2txbrxnea.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yopsvtek.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2quwbuskm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2klcfmkax.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lsjqdanu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tchfyypx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2hgfijrbf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2vqcbikzm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2wgetlycl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2nbujimuf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gzfkddmj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2cjfhsrnn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2mtkoiukk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2wfdkdxnt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ovwrnkbt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2cwxzwwpz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nqeeeiup.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ruausysy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2emvdaxjt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkphvwwn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xpxuqwnl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2dqugvjwi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gutskzct.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2athkverm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpbzkbnu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2puqboglh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2pkbkjgfj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2mkjerrvk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2kgnqvplo.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2kmjudsnh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2iwsgvqob.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2trmewrtk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2litnyryl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cozlsorh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvdatdnb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ardufdbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ynzkotgt.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jgdjuuvo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2lbdcdvwp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykqesfve.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vevzrumv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ntoxeqev.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2afphydsj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2briealec.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dpgpjqri.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qidinvir.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2oeilqpla.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xwgogetw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgclvgkn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fvilbhwp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kwdenyil.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nzrbwqag.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2syfisllb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xrvbxssl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kzaxridt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qtntriry.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qmkqrmwz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2drhvupxf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uthveemh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gnrpmhzs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2skkxhpkv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tlrnupkw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2artxbzye.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ayunrzmj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2olotqdqv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wfjqghke.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjfqyook.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2erorpmjj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxvxrzri.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2hqcsrczb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2fvyikiam.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ksnjqone.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwyzfkcw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fvawagwv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xenolgpg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2hlhygaoq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwfnefij.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkrcomjq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2autvbygm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fpijetab.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ufoeuswe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wglaovfr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2mrbgefho.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xufgendk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2onulllkz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2olzfdzui.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hylzjwye.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2cmemlkja.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2tcxpsdhx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2howojoae.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2goebhbod.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2eiwqyokc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wjtkogda.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovecoudz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zrjrtoka.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tyxduksf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dedivoeo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2noxlhaxh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kclgwlzh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tsmldjqk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xudfunit.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2xujdkwti.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ppjcoimd.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2guuxvpgx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kskkeuud.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zjtbfuxt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bllmvweh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2uvbwxpin.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qasyaswu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2dalmzcho.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2bvewhcik.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ompyxdgw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddozlphs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xizrqnpy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aahrfdnd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gyaisytq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ncmvfebg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdztgguk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ehibsutp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ickdolbo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cwmglyah.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ilstnxfg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pkdnriqt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2dajtbmkc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rtluxtra.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dvzivwri.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2nzgefrcy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2mixjapqy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2szcspwir.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ydznvrji.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rbepfcoc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tbbuqits.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2prgpdbkl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2fetjiloi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2sagepxvg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nopghtta.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ypovzwio.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2svrlvqzc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hqusizco.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2geihxhaj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yevzimyk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tjeiglni.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hzqstpth.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2bhwwwjxv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ebmhtiqj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2gosubcgq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tzzcunzl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2rclqjfha.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qnlofagj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zcddmdis.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2rppswgql.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2kflwonql.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2dhrfynsz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2julrilrp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ofcbzyrt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2khptyxfj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2okgapmjm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zklbqbnp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dksypcdd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pyjiwxze.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2nvntauoe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2aduflcgu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nuwftltf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2pclitpvz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vewdbzoc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2koxwgafj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dtplqrgl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ehontmrq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2czxfgefz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vqsgambs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cppghqsj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qbuuilei.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zskbayhj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2njiqodrg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2teaebpcv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hfizzasx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pyxavmbf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gorwddwu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2kflkmqni.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2stkuuejy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2invofuka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbvbnhov.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kxujznei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tidbfyob.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ysdlvdgm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lrgabouk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngytrqoq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bdkummxq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jilibdsh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2suezejaf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2hupqurlt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2yequyrrm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gejcawfz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2msjhxgou.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vsbllcqe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yycblmkj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kjwlozrc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nwbayofr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zjrpsqma.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2opgwnpot.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2pwffnbjq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2guwbbscd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rjqaxbbs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2qgiccvwm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2gffvkssa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fubotcvw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjfvvkqi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rohytunw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2uopphokh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2hwhrrlit.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2zcavvakb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ybpzfhxr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2zhidquuz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tggyxjyx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bbrdlelq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2icewqykh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2eoiqtout.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rwiayqbx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qgiadbrk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ulkddvxv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2uytoxgvl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2koysukxg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2thntwhkz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gsdnonyw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tmhhrtrk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2trmytmeq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fzvdcfea.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2rjnwzxai.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2cyqsphds.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zorexdtv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2uqayfjnm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rhcbuaxu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2alsbvuor.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dvmqlqul.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cormoood.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kusumprw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2acehcmmp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yhjvytzq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rwtzadfk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2oqhasszf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vttkpjtp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2abatyekc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wyelpbfm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dzmcjkkv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2eodehjas.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ftljpzwh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2dlxpoaul.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ymmldcgs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ycsxskih.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2cfnpxtqu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkxedltz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nterigdy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2yzfvjddy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2hzvrgdoy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jwiymbnl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lleziuai.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ospnippq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xbqxvyhb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vrfofhdn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uhkntccs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mpkzhpbl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fwnlyree.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2gitpojsk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tcmzvrdd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vuptxnom.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vahjgybm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2gdsgwqbc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2gfaujszq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2imfasjez.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nrqpryxn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hdbdxvhb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jmmbxtky.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2yfenrnuo.html


<!-- 参考信息 -->