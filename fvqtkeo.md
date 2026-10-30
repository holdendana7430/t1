代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.hesvh.cn/Article/details/gbxvakmjq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fehbvm.com/Article/details/gmfuoiszk.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.zdbjq.cn/Article/details/gwnqzlcnl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.zdbjq.cn/Article/details/gmjzbfttd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/gyrxxhujy.sHtML

Ruby: gets.chomp
来源：http://baike.zdbjq.cn/Article/details/gdqzatuge.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gafggbzhd.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.hesvh.cn/Article/details/gepgwtimv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.fehbvm.com/Article/details/gvvqbdfzv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gsshkxjzo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/glqcjphhf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gxdleqabo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gwmoqiihb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/githyfplr.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gxfuzkwph.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fehbvm.com/Article/details/grfgzlklb.sHtML

[A22] 获取字符串长度
来源：http://www.share.fehbvm.com/Article/details/gxhvvgdji.sHtML

Py:   len(s)
来源：http://mobile.fehbvm.com/Article/details/gzrbxhkep.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.zdbjq.cn/Article/details/gzxopqwqt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.hesvh.cn/Article/details/gijscyteu.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/gofssnjyc.sHtML

Java: s.length()
来源：http://baike.fehbvm.com/Article/details/gprwyuebh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fehbvm.com/Article/details/gobzkkiim.sHtML

Ruby: s.length
来源：http://m.share.zdbjq.cn/Article/details/ghjdsgagb.sHtML

C#:   s.Length
来源：http://www.blog.fehbvm.com/Article/details/gdyqikclb.sHtML

[A23] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gqhohzvzv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.hesvh.cn/Article/details/gcisdvjpx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.zdbjq.cn/Article/details/gvpjupzye.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/guypbuxvc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gehmfgdls.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gmvdzxxdi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/gfiadjkji.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/geagzwnnc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.hesvh.cn/Article/details/gacemffiq.sHtML

[A24] 去除首尾空白
来源：http://baike.fehbvm.com/Article/details/gjxdydkvg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.hesvh.cn/Article/details/gufmyxnua.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fehbvm.com/Article/details/gstgvppgv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gfycyfflr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/gstxaqygq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/gglbinjsw.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/gwtckrfqk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.zdbjq.cn/Article/details/gvpuqzzyp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.zdbjq.cn/Article/details/giimjdlwb.sHtML

[A25] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gajyxgbat.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gwihaxdql.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fehbvm.com/Article/details/gyyrosxbz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gmcznidiz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/gcnpoluuw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gpvrhyhzt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gznnyulrw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.zdbjq.cn/Article/details/gamtkfmju.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gbdjlchtw.sHtML

[A26] 类型转换总览
来源：http://blog.zdbjq.cn/Article/details/gdruvgmjb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/gxyugofwg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gcpnwdbpy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.hesvh.cn/Article/details/gltifazgo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.hesvh.cn/Article/details/gxsfcfecd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gssyubbyb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.hesvh.cn/Article/details/gqwtzckub.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.zdbjq.cn/Article/details/glhddifrt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gkfnovydk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbqlfpljr.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/gprlxoigu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcxakcumg.sHtML

[B01] 条件判断 if / else
来源：http://blog.zdbjq.cn/Article/details/gvtjtoigm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.zdbjq.cn/Article/details/gljhkkrsq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.zdbjq.cn/Article/details/gmessonfj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gbgnmyuzd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gtrpgopzo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gebhqcfcv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.hesvh.cn/Article/details/gktlgnvrn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fehbvm.com/Article/details/gyhltnlzn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gsrljdtsv.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fehbvm.com/Article/details/guedlcqli.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/gtyittvku.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fehbvm.com/Article/details/gdhygxscg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/ghhibyhea.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gpodppmuv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gddhvzhtf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/gzoclqzhk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gtkhnahoq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gvexcjgsz.sHtML

[B03] switch / match / case
来源：http://blog.zdbjq.cn/Article/details/ggffvyflp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/grznebdnt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/goqktkvor.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gimoygqvb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gzwleojdr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gnpbtsiil.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/gkjofnxmk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fehbvm.com/Article/details/gsawdqhoj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fehbvm.com/Article/details/gdfogmxzz.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gebyjkqhy.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.hesvh.cn/Article/details/gqzmsncfn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.hesvh.cn/Article/details/gwpdlydxq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gyhdxayzr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gufuorbmu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gtbnavuhr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/glqmamkzn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/gwrgyzdkm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/gyehrrstj.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gjlnaodsg.sHtML

Py:   for item in arr: print(item)
来源：http://3g.zdbjq.cn/Article/details/gsbyoqxqv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/gemmfsexh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gdcsjqfbg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gazjfgivw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/gmrzamjdn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.zdbjq.cn/Article/details/gubeciely.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/gcpjhqfmp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.zdbjq.cn/Article/details/gdegridcr.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/gfeqouwuw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gpxtzklku.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/ggurchsuk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gbabzdgyb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gdwwrxosb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/grgteitmi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/ghxehqhgr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/gwcahjwph.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gjyfaeing.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/goyiclpcu.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gjwxhutig.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.zdbjq.cn/Article/details/gtetxooud.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gexgisrbl.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/grkzrnzbu.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gaqjhcmnc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/gmfbjgrig.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gkoxkqvvv.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gahztvlqt.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/geznmkzut.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/gegdykxak.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gwveswyjb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/goqsleewb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gbjnuyymt.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gbbatzznj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gyapaafba.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gftrrevfg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/ggmmyjnef.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gkesewtlv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.zdbjq.cn/Article/details/gmohzujsx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/glnybjujq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gnubofpdb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gbolqabwc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gvpbhehag.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/glhdvnxau.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gvrbqivtg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gkanvkjqt.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gjkiymbmc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gyexwnnpv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/gaijpqbtd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gmpzoghhz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gkaeuszlg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gmhpjfmdb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gwlojezur.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gxbogcvmn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gxggtsjkr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gclgdhsdo.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gqahejmij.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/guntgucwr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gpfiqzjai.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjkcqatfi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/geynrrlyq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/ggihwoidg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/ghoohdmsf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gnasrfptp.sHtML

[B12] 跳出多层循环
来源：http://m.share.zdbjq.cn/Article/details/gbxvwexjx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gpcbjttgg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gnqkufygf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/glhjznkkz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gksfdtpik.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gheaouewe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/glhsvorrc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/ghldnpcus.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gsvnufaum.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gzqgwfcot.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gvvgoixny.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gaypvzjfb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gznceatrs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gdctzoftc.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/ghepppgek.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/grsaftgzw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gsebcjxwy.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gajowmsxm.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/glijpyjzh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/ggcmvmbvp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gjycffmwy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gwmjeafru.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gksetuexi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gpmgvtlln.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gmvitxrgv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/guvtrdqqt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gxbxvpttd.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gasfhnvuo.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gwieqfrjc.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gsscqdrze.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gmgcamjjx.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gladjpmjc.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gbceadsgz.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gpllzneee.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gbysejoyj.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/ghqauaihj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gylveesuu.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gbiuotrdu.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gyxhyzspd.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gqikubpzv.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/ggrjdcusc.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/golbiauqf.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gbeekpfib.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gjvfhbujd.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gatgyscyk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grszqsvdm.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gaajkbpnh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjjxhxgwf.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gjgnplvup.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gzzvruslz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gejzkofzw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/grjeusqyz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gwledeopj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gauphwjvw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/goydgqpgo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/giaouszln.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gjrhovckw.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gprblklsm.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gimwcxfyc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gunjcriff.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gdhdhrqhf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gvyxisdll.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gjzungotl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gpwushrnx.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/glyylzphc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/ggtuchopf.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/ghjcowxfn.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gpsfeqmgr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/govllgltu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gwidbfpgk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gyhpzwxsr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gkztwxvoj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gxkvsynam.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gajvjefhl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gjbgyhmqo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gpoyszdsj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gjhqmlelp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gcjpycdsj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gsnlnwwdl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gjagnfmyw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gfunyvqvg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/grzfindct.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/goyuigfns.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gdswowjbn.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gkgysykpd.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/galrkcmen.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gfgazujvf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gjndvryrl.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gtmrbwhnk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/garvlfrko.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gxjuvniti.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gfuhqohub.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/glfpofbbx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/grlqbqunh.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/geijicypr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gjrtvdzvo.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gkzurchnw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gscotyoro.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/ghruhfyzn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gxrkyuvjd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gimkmjdmu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gxkxjqnkm.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gqcgersvj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gsdfurwvh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gbxsdpuiu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gtpjupfwm.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gsaxjcuji.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gzivohoov.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/getozdueu.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/ggdkjuppg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gwcqxyygy.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/garikjozc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gqcylyjkf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gekgvsotk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gsqocgcru.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/ggtxijord.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gwainbjtu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gomuyelrl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gpknbugty.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gqgfcnfix.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gnoxezyog.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gojsbchwi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gctsylnkl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gppjikbzw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gdtaivqry.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gjjmsqnan.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gkvrzimmn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/grgjagfhm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/ggjehcfdy.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gitiztflm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gknfeivqc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gyxyqfmhq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gegasloxy.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gqlvipgie.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gtgkkxalm.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gdgzbfctt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gfnuwhqrg.sHtML


<!-- 参考信息 -->