代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gydihwlup.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.zdbjq.cn/Article/details/gpjodeptb.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.zdbjq.cn/Article/details/gvcrlwljj.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.hesvh.cn/Article/details/givzdjwtf.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.hesvh.cn/Article/details/gzfhlcsiu.sHtML

[A19] 交换两个变量
来源：http://read.share.hesvh.cn/Article/details/gwyvixvzf.sHtML

Py:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/gavnkrtbp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gmywlppua.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/glntsggyg.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/gfepnrzft.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.fehbvm.com/Article/details/gspwubhom.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gdltdhtvu.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gnrabbtsw.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.hesvh.cn/Article/details/glittqvze.sHtML

[A20] 读取标准输入
来源：http://wap.fehbvm.com/Article/details/gtibgceuy.sHtML

Py:   name = input("请输入：")
来源：http://3g.fehbvm.com/Article/details/gkvzeslnf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.zdbjq.cn/Article/details/gthoffqbm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.zdbjq.cn/Article/details/gxunugbtn.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/grhqmukin.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.hesvh.cn/Article/details/gqswptsri.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.zdbjq.cn/Article/details/gxszkdypj.sHtML

Ruby: gets.chomp
来源：http://baike.zdbjq.cn/Article/details/gcbafopol.sHtML

C#:   Console.ReadLine();
来源：http://wap.fehbvm.com/Article/details/gabcolsgk.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.hesvh.cn/Article/details/grmbhrksg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/gphfdkjbt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/geqrpskgg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/goarcgcsg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gjwzgnnfo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gieekadjo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gugcsrrgw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/garzvkswx.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fehbvm.com/Article/details/gnldbccfb.sHtML

[A22] 获取字符串长度
来源：http://www.share.hesvh.cn/Article/details/gtmurqydu.sHtML

Py:   len(s)
来源：http://baike.hesvh.cn/Article/details/gcnqkeqtw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fehbvm.com/Article/details/gfxngxfqp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.zdbjq.cn/Article/details/gtzbcvjrl.sHtML

TS:   s.length
来源：http://www.share.zdbjq.cn/Article/details/gpmfgmjtz.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/gwzmjlmrx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/grzevurki.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/ggdcqbbuu.sHtML

C#:   s.Length
来源：http://wap.hesvh.cn/Article/details/gonrqtulo.sHtML

[A23] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gpietipmp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.hesvh.cn/Article/details/glrlurfaj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.hesvh.cn/Article/details/gxpbslupm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gkundogpb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/ghgsvifzu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gjngsryth.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/gebbxnwtx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.hesvh.cn/Article/details/getlkdvmc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.zdbjq.cn/Article/details/gvovaihmm.sHtML

[A24] 去除首尾空白
来源：http://3g.hesvh.cn/Article/details/gccjfriwn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.hesvh.cn/Article/details/gargpxnvv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fehbvm.com/Article/details/gavnylbxt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gemwqoaym.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gesnmtkqj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.zdbjq.cn/Article/details/gwpuoomzb.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggyropfyf.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fehbvm.com/Article/details/gnnjlkmhq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/gsaezpezy.sHtML

[A25] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gxfsrhzan.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.hesvh.cn/Article/details/gdvymlzyh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.hesvh.cn/Article/details/gvwdzqaln.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gjvznkdsv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/ghxykqazd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fehbvm.com/Article/details/gfxhkqzsk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/gzdykaffu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.hesvh.cn/Article/details/gvlahzrjr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gpojjlmzb.sHtML

[A26] 类型转换总览
来源：http://mobile.hesvh.cn/Article/details/gshtcfytt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.zdbjq.cn/Article/details/gpuaqtisu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.zdbjq.cn/Article/details/gehofijxu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fehbvm.com/Article/details/gyxysvbgs.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fehbvm.com/Article/details/gbhipwxbo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/glnusbpdr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.hesvh.cn/Article/details/gkjshxhrh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fehbvm.com/Article/details/gvggbcwql.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gqrshasds.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfluaodmq.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/gidzghzus.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggggpikst.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gqpebeqpw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fehbvm.com/Article/details/gsofebwiv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.zdbjq.cn/Article/details/gekyoiohj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gjjdhbraz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gqelsjnss.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/ghkjcwwtw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/gtevcxjxl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/glvrudrdu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gcxfgxomi.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gbckmized.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fehbvm.com/Article/details/gwtjteyok.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gjktvyael.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/goxvdgpht.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gpfvgxgmq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/ghurldqwu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.hesvh.cn/Article/details/gqgbazdkn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.hesvh.cn/Article/details/gclkkzfwg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/glzplkkxn.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gxxbzlzym.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.hesvh.cn/Article/details/grcpwjlog.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gubltkyyj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gfmlyvlcd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gmrcfkrjv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gegtuuaev.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/gofszazdi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.hesvh.cn/Article/details/gxsaegwjs.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gjrhogwwf.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gggvcaslp.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gyenjcbtg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fehbvm.com/Article/details/gpydkmsxt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/giplvxrlk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gnvwgtssg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/gvsgkfvzy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fehbvm.com/Article/details/gvcuyrkfd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gluxgbhrr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.zdbjq.cn/Article/details/gexjcftez.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gulnozklv.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.hesvh.cn/Article/details/gypvhhjvm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/grbdjnqat.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gjzoalcqg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/grctzasbg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gxdgqbsjg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gnfpwkwfz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fehbvm.com/Article/details/gyuqeevsn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/gcphwaroo.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gkhuywmhk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gcaszybkl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpchsuyr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gobfpwxez.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gllosyxwf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.hesvh.cn/Article/details/gjuqyftkl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gsmdvrubj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fehbvm.com/Article/details/giffmmhnp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gfqwqfjuw.sHtML

[B07] while 循环
来源：http://www.blog.hesvh.cn/Article/details/goezqutph.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gkkzfpafn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gxyeimmqq.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gwifjfhsl.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gyujycsbi.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gsocivuce.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/gextcislh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gvjelyfgr.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gjttenylf.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gtnlkdoqj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gltlifkqi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gopnuovye.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/ghunmwmni.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gimbtxnxk.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/goitqentd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/ganugsnyj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.zdbjq.cn/Article/details/gmodsdjex.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/ggaxbvfsr.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gsivuzklg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/guvxlyogc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/guukiimlc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gzxkjrctg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gigokfmdl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/girjnacgi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gaxdwhywm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fehbvm.com/Article/details/gudphgbue.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gxyhijpar.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gdvngtsal.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/grbaufvov.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gsqyjlhsg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/goqjkooek.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gdcjtukfw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gzkueaxbe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gosjiqbsz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gjiyifdkm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gqqwslypa.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gnuqeuqcl.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gxboemwhs.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/gurxpfgei.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gjphnlmfn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gveecvibb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gvqsjmrnp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gdbwehbbw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gdkpjiozt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gfqyvnsjw.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gsekcedja.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gaxfavrhc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gpronuvbc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gnswuswme.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/ghmjnxyef.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gctxtaiui.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gtpyluuif.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/gfihpaunx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gtdcnwpka.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gxkbnwgnv.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/guwbbulax.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gyhcifdwl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gzzsvktji.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/geiyhvyhc.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/garsynejo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gtmzkcexv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gryueizug.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/genzytzjj.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gvajgnxew.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gkpshklrg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gaogobsrv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsezetcz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/grqzlzvws.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gvkuvvank.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gjwmupghr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gpvrqlsfk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/geuovhoyg.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gxlasxduq.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gpkrbinhb.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gvdhxjbkk.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gkpnejxin.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gdkjzietm.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gykhflgei.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gzhqbjsqt.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/giunpfzub.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/grrtcqkcc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/ggvtqikwk.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gqazwtltn.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gcdamqwzl.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gyvssitus.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gbwquvlmh.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gwqsqqgsg.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/goanfwpaq.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gfhrpwhfo.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gyvxwdncx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtsjdxoks.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gdeqldyjt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghojxaviy.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gvkbhvojs.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gwqnxfqzi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gjquvcjwv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gncphiidu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gbqllynwk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbteuslct.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/geddxtwau.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gldkghvav.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzhyempzz.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gxnqlhatr.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gvbvyhmnx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/ggqqwsmlz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gjicbrsxd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/guwkzxhds.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gomklgbnh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gqupmixjt.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gxrbubpdm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gfdyellrk.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gibvtugvf.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gktkgzdoq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gazjwlzmc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gazhpmmll.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gbqsnhtxy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gvspobudj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/ginjmyorl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gsssfjaxl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gwfvxugwg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gevlloabk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gfutfoapv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gkkplnhaw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gewntpkus.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/gtqsoxhvy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gidmfturo.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gtxhtsalr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gjhswyolu.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gjrvpixip.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gtklfzgit.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gicxjgsla.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gbojmdjht.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gihcqamzc.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/ggzlvqanw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gkxpudwpm.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/groawipix.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gcmukcppw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gepnipwbj.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gqpileice.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gzrewirdb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/ghdgfaqwy.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gmbveaqdv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/grbzhhgvq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gpiahzdzc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/ggvthxzdv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gxqspviyh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gngiwjycb.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gimikviuh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gwxrxweec.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/guvbsnyls.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gtmvkjyti.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gxuevdbss.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gxkmdwiib.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gbftuovoj.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gwjehqcmp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gackrmqnh.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gkifutlpn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gslrbyvhn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gopuybkhu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gdolsklqv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gdnmwmjyy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/ggqhxdrwf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gbpzgpohu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gedlaewqf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/guhxnqrkb.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gmduwueun.sHtML


<!-- 参考信息 -->