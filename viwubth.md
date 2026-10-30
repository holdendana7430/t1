代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gxkegysrl.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/gvntawgbe.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.hesvh.cn/Article/details/gvpoarsjl.sHtML

Go:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/gkqikdjly.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gjrxbwxlf.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fehbvm.com/Article/details/gmzqazqvq.sHtML

[A20] 读取标准输入
来源：http://baike.zdbjq.cn/Article/details/gafalktru.sHtML

Py:   name = input("请输入：")
来源：http://mobile.zdbjq.cn/Article/details/gidvbblkd.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fehbvm.com/Article/details/gshvplfuu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/gtasibdkm.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/ggrbfbnjn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.zdbjq.cn/Article/details/gxkcvdywx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fehbvm.com/Article/details/gphfiezom.sHtML

Ruby: gets.chomp
来源：http://www.blog.hesvh.cn/Article/details/gsnbkynjm.sHtML

C#:   Console.ReadLine();
来源：http://www.share.hesvh.cn/Article/details/gadwbzwty.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fehbvm.com/Article/details/gflaopchl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.zdbjq.cn/Article/details/gevmffydm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/glakecfij.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/geakdymxr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gueardolj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gbrkekvxi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/glodujxba.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gjzspawxu.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.hesvh.cn/Article/details/gfgezecsy.sHtML

[A22] 获取字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gsijcsmyx.sHtML

Py:   len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdccaruda.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/glaszmgyd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fehbvm.com/Article/details/gkldxcrla.sHtML

TS:   s.length
来源：http://www.m.share.hesvh.cn/Article/details/gjbjixjct.sHtML

Java: s.length()
来源：http://blog.fehbvm.com/Article/details/gqgxmwlnu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/gmihxajpc.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/gwlycikgl.sHtML

C#:   s.Length
来源：http://mobile.hesvh.cn/Article/details/guugarnnj.sHtML

[A23] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/ggkmmqugd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gbujtzoiy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.hesvh.cn/Article/details/gmjtznoaa.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gyzlvyksf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/goeqpmuag.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gametgone.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.hesvh.cn/Article/details/gxbusenwo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gubcdcshz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fehbvm.com/Article/details/gdunulrjg.sHtML

[A24] 去除首尾空白
来源：http://mobile.hesvh.cn/Article/details/gjmcxtilw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.hesvh.cn/Article/details/guxpnixow.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/golbvtzkw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gnizeaqiq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gwdjpstke.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fehbvm.com/Article/details/gihfpiuep.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/gmhpmnafo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.zdbjq.cn/Article/details/galjpurdz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gpukfnhjm.sHtML

[A25] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gwkicihhp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/gzgrmzlsv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/ggdnjbsci.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/gpdjhtprb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gmjalojye.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.hesvh.cn/Article/details/goiiadyqk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gipmgrdrf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fehbvm.com/Article/details/gjodnwweg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gcnfeyqqq.sHtML

[A26] 类型转换总览
来源：http://read.share.hesvh.cn/Article/details/gasvsfled.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.zdbjq.cn/Article/details/gprygwxew.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gdojaxefe.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/ggfnzglnm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/gwgwbytcg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.hesvh.cn/Article/details/geqzneowy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/gcikpppfx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.zdbjq.cn/Article/details/gyuubithl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/guewbptne.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyqlgaseo.sHtML

B. 流程控制
来源：http://www.blog.zdbjq.cn/Article/details/grrshqggr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqjygdkek.sHtML

[B01] 条件判断 if / else
来源：http://baike.hesvh.cn/Article/details/goedgigru.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gepnezgcr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.hesvh.cn/Article/details/giordhfoz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gaisqupqk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gwhvrocvi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gxhfepvyj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.hesvh.cn/Article/details/gixmdngog.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.hesvh.cn/Article/details/glrhuafru.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gyfnnouau.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fehbvm.com/Article/details/gutawkhwm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.zdbjq.cn/Article/details/glqgwbtkw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/grfxtcmjm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gxzkjwaye.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gskwrthft.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/grrbalbjl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fehbvm.com/Article/details/gfbvbqtcp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gcpucegcf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gmvsmrykt.sHtML

[B03] switch / match / case
来源：http://baike.hesvh.cn/Article/details/gmuvrotur.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fehbvm.com/Article/details/gvstrvvcz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/godrmimqz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gqjbjungs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gaupjimqy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gzegajxry.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fehbvm.com/Article/details/glosflcep.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/gjgratpbl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/grxlaktet.sHtML

[B04] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/ghbzacpbj.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/gekbbcehs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/geothdfvy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gtvopvjzm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyobedrdr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/gqtlbymyp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/ghlhcjhmy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fehbvm.com/Article/details/gzsoesjfi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/gqnhllwvm.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gkosiwopt.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.zdbjq.cn/Article/details/gmvbckklg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.hesvh.cn/Article/details/ghksesgen.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gbyiwnkhe.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gqtplvbic.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gnnbheghp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gwooqpirj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.hesvh.cn/Article/details/gsozcrzwv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.hesvh.cn/Article/details/gwuwaggeo.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/gzzsvqvvn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/grzoxknae.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gwnxndhoq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/glffumsam.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gvtiqomfc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/guieapqbs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gayrkksho.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/geovliwkz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gfwkqdjuw.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gcqtukgfb.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/gewekxfup.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gvekrmtzq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gxribvovc.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/grdpwaton.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gvpcxnqbk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gmqrpdlbn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.hesvh.cn/Article/details/gkvjvvbtg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/glecpjwsy.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gdvdjvhcy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/glhaxttyp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/garzukvrv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gfsrblmxq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gewhkgpha.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/glxgbmaul.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gcfshdggi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/ghgpbpxub.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/geqorgvzv.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gvqvjzuer.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/grkecvafl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/glnkfplnk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gugbhibpk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gvhfvtfte.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gpgvkksle.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/guxcwawdd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfgmequr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/giyuzujpp.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gqtzdbiiw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gbtqvwtmq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gwadolcgw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gtelvrqaq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gnnsrnshl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gkhtzdzlc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gxfiqyjrd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/giswpqxyg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gzwgzewbh.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gtsdbnucs.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gvydfuwir.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/gabmypmqw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gqkjoyxxl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gegjcqnnw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdcjzwwoa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gsdyyculs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/glqdlaprd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gruhpkhsc.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gxvguqryw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gtfeizwqw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gtxfmumab.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gduxnuvqe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gzjookvfo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/ghmwscite.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gtcoburta.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gbivemfov.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gyhyeatum.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gscnnrwxy.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gxgjsanpa.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/ggnwrrygw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gmiunqfhc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/ghzitcblf.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gqetngmox.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gnhnnfmvb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/glkhgmpqh.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gjejryevc.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/glirbstij.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gafjhgvao.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gqczziycc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gfurpaimi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/ggfhrdmbv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gyndkkaym.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gppxuqapm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/ggzddtooq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/ghsbytxsu.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gnpzbitee.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gjjsrerzx.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gkiwtlkcd.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gmfxqfgmy.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gcfgbbdqz.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gftbxbvig.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gnhnooafc.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gdhbbypkz.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gxhowzlox.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gvlluizuv.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/grtokrfzr.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gjdqzlrwm.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gdrxfpmfl.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gbuhmepuc.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gfrrddjkn.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/ggilforap.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gdottdnte.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gthpmfszl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyjvqzzye.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gmdrrevtu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcehbadho.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gqtjcsynt.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gqqtnaokv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gfhvyzwir.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ggrzbpjpf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gymlwrmwx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gnhehvbar.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/guzvjhnbd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gmbrygvoa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gjthewsog.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gtrkgigpa.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gffobcfbb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/goyonhiuf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gahjvrait.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gannrgakz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/ggqhribkg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/ghmgfwukb.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gjfsedgmm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gfehhdhqj.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gxkkcfkgw.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/ggeciiybb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gtvmsozwp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/glojbvmlk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gbzophqcs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gyfelqenw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/grwrnkpcr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gjdhfyfpj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/ghnddpqty.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gmbuamzgx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gqowfkqgp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gbowzqaqf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gezzxsmiq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/guitmjxxy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gkqbdudoa.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gxjaxzati.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjnmkbhkw.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gbwunegpd.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gvprmukvc.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/grexfxhyg.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gskgqdqqy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gphepvkmn.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gyymkkafw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gziojejns.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gnvnoqncf.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gbinswnsp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gpfjeqypl.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gvdprnuvj.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gqikidzoe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gmwoydnwy.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gamichuvu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gxwzfeoxr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gjgmvzwnf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gldkbplhy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gamezgpsu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gdmskyzcu.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/ghxcdqwfu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gnmyicdte.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/ggkofksmo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gxkaeiifs.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gutkhyrkg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gdmkgwvtm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gaghelrjs.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gshuyguac.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/grrqbuqtt.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gomwxcrsr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gzrklfgda.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gbxxwdegt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ggtftlxkb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/ghrrowdpd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/ggkxsgrnb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/glglmkpxa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/ggmyqkoij.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gbiokppul.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gdyburfum.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gkaoucncr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gayxqaptj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gjtymuucz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gzhmydsfa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gohbeittu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gnzafgzvo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gxamwhdes.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gmvjxxbxf.sHtML


<!-- 参考信息 -->