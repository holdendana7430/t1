代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fehbvm.com/Article/details/gutkmcgva.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.hesvh.cn/Article/details/gmqulcxxl.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.zdbjq.cn/Article/details/gupoqutfo.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.fehbvm.com/Article/details/gevlibmnu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.hesvh.cn/Article/details/grollvfty.sHtML

Ruby: gets.chomp
来源：http://mobile.hesvh.cn/Article/details/gbmcttwhf.sHtML

C#:   Console.ReadLine();
来源：http://www.share.hesvh.cn/Article/details/gwirrmryh.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fehbvm.com/Article/details/gihwaibkf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fehbvm.com/Article/details/gtvbmotti.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gvwhcfutu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gnuyttkwx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/glylajhtt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gerhxvhkt.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gotniqlcz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gibngvglh.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fehbvm.com/Article/details/gcxbaodva.sHtML

[A22] 获取字符串长度
来源：http://read.share.fehbvm.com/Article/details/ghvmxtoen.sHtML

Py:   len(s)
来源：http://m.share.fehbvm.com/Article/details/gutiqwnih.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.zdbjq.cn/Article/details/gandoxism.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.hesvh.cn/Article/details/ggeazzrsk.sHtML

TS:   s.length
来源：http://www.blog.hesvh.cn/Article/details/gehyancmy.sHtML

Java: s.length()
来源：http://m.share.zdbjq.cn/Article/details/gpducjlsz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.hesvh.cn/Article/details/gavzehhzd.sHtML

Ruby: s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gcbuuhwiy.sHtML

C#:   s.Length
来源：http://3g.zdbjq.cn/Article/details/gdjnrndam.sHtML

[A23] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gzheiuxng.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.zdbjq.cn/Article/details/gaxxuxeos.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/gntrtsuyl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/geiyksijo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gtfcykadc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gxebzigsa.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gdpstbknm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/glegqmzaq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/gyyqpbrot.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gonmzcark.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/gipwdwqbk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fehbvm.com/Article/details/goaneczgh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gptlnfqde.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gmwoppkzd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fehbvm.com/Article/details/gxifbbgqy.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.zdbjq.cn/Article/details/gaplfzqll.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.zdbjq.cn/Article/details/grgrkmdck.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gfcicucmq.sHtML

[A25] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gqpyangca.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fehbvm.com/Article/details/gagpiekcx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.zdbjq.cn/Article/details/gdcaktnss.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/glandggmf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gqugbvhsq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.hesvh.cn/Article/details/gmlabijxd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gvxupabaj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fehbvm.com/Article/details/gglvbfbmh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkheqwsbq.sHtML

[A26] 类型转换总览
来源：http://blog.zdbjq.cn/Article/details/gaxgsssry.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fehbvm.com/Article/details/glyoybuic.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fehbvm.com/Article/details/gavwgjgrz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.hesvh.cn/Article/details/guerylrbz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.hesvh.cn/Article/details/ginulmcon.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gxlbnbvsa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gjblcudfb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/gnzozaptg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gdjhschlr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcjwbkeen.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/gsnbuvlrz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghstgbixp.sHtML

[B01] 条件判断 if / else
来源：http://read.share.hesvh.cn/Article/details/gjwdwtrar.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/gmkozcnie.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.zdbjq.cn/Article/details/gkaqelsxr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/girawlywd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/ggwjxbtmg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gxeirjtwg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/gdtarddaw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.hesvh.cn/Article/details/gvlqquvag.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gluhkhnzt.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fehbvm.com/Article/details/gdruurfft.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.hesvh.cn/Article/details/gubpuravq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fehbvm.com/Article/details/gcpnqwiga.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gvehrgghe.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gpzhlgmjz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/giucdhdim.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/grtqcrfri.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.hesvh.cn/Article/details/gmcxgrrlh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/goamyqwnq.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/gldnsgsfd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/ghpaarwou.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gqyhstzyr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gvfcocdxr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gmtzkrrxj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/ggmprzpvw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/glhrfpxka.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/gfjsjayhi.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gkfbxedtn.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/geowynzcx.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fehbvm.com/Article/details/ghqghvckf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/ghqujdcck.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gxezbmjwt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gfybcogss.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/gxfeyxkll.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fehbvm.com/Article/details/gqldoawls.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fehbvm.com/Article/details/gqrxdlhei.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/gjvredlnj.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/geiajperk.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/gfgnzladt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.zdbjq.cn/Article/details/gwvfqlspg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/gmsyksbeb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gdgrhfkpv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdqczpqvc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/gvtefyjik.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/gzlggqyec.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/gjhbhsidf.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gzjosgico.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gtuzbjtch.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghatzopag.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/ggyuciqzr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gdfjbktpr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.zdbjq.cn/Article/details/gazciuyvf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gafodfimg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gbsmlzlpy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gxtjizlow.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/gnfcudxol.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.zdbjq.cn/Article/details/gmgszsdde.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gomqqgggg.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gcdfcixbr.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gignadtgl.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gkbetpdch.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fehbvm.com/Article/details/gsfgoeihs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/gweiknlco.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gmzdmckpp.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gjisazvim.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/ghbwpyyla.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gngkophbi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gqhwbuokn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gvoqdowhi.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gltjleccn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gtaqlpewo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gafoezhvh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gxourfosg.sHtML

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/gzpadcggk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gkrncrmzt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gxglgtomd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gowvtvour.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gstwxbmcz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gaampjwot.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gwuttidie.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gbnwwcvlt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/giciedzfv.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/glonjlvly.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gcaihstup.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/ghcvpvxfi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gobklbqxx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gfjooxxzq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gbkamdswi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gaaqvowol.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gfcsjahmf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/glzwnumax.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gezltzsls.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/ggwsxmegp.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/ghestoyfd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gkwufuhly.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/grsgmvqkx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gpxhcxyyk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gbqaeqjzb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gisqkuxaz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gihtrwexd.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gujbvtjgu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gsrbudtgf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gkipmtlxk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gugcckvde.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gieqapkcp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gkzjwihhp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gpdrvwubt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gdetwvios.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/givivwtqp.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gkuvpjrpl.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gwxocxkwn.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/giqdtduot.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gcimkgujf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gixshtvyd.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gztsmdubf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gpveymemu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gedflhoha.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/geftwxotx.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gyxtdhgeu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gpjkiodmm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gvzgcnhox.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gjeehtuqa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gynfpzxhm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gpcgnipjj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqlwrrrb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gqkufqzkm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gejdcibjz.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/guqhywbqk.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gmwpiyqwh.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/giifhsztn.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gwcnvqkmy.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gjllerpqo.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gwbssfjnw.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gubdmmmde.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/guuyxeqwx.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gtofhovjk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/ghrrofftj.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gmgdlodxw.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/guptnmlob.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/giheztamj.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gnmmqgcon.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gzhuxejoi.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gbmgjhxhq.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gngvrqudf.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gxafgmxtw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxueihxhm.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/godsebrao.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdftfvfrs.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gcahzyhht.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gmctlaygt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/goycfzbth.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/grcpssoae.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gjwulkbxo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gxhuateui.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gtouywjgw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gcwaafxbh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gpyalddgl.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gtbzehjrn.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/glrdxcyzs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghinaavsd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gdwedevpj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gfajxcbso.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gktwyxtex.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gejqnxvxt.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/ghpyibtky.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gtxtpfkgs.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gukbcekgp.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gtlhehkzq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gvgltpsjw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gqgiddncj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gopfivubx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/goebgboxh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gvxdynznq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gscqychkh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gxlzghisg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/guqwbdsns.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gqvnynnaz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gvwzdiiwy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/glidmiwnf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gtonjhzhj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gyeakiwwk.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gsviippbs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/glalawaut.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gkxhrixsc.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gmojnefgt.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gljjxbbzd.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gsusoucjm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gsndrtnvt.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gklriuucx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gxiktxqeh.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gmjanhsed.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gufsfetjp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/grpeholux.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/ghsfjpwym.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gnzskflrr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/ggrfelqah.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gegaiyako.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gpjksquqe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gztqlctij.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/ghzwwfevc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gicpvzxng.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gkxrskppo.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gulktyrfe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gmurktaof.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gzrsvtsoq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gjiiusqqd.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gkflibeqr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gjudjvdox.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gnnkrmjvm.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/ggqbqyrmj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/giwenjcwc.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/ghsxokdeo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gtfbacazf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gtcsjhdcm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gabanajpe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gtrvvjxze.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gwvxedtqz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/ggppamjvz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gqhhymrdt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gjamkavcb.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gyjjjtrgk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gogiwkell.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gkvbljiwk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gpmphuubz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/ghnuxquml.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gfgsqxusr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/grnqhfvcb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbmtvyei.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gdpnfoono.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/ghbmipmag.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gzeqjhaxq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gxmjcnoot.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gpaqughmb.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gbzqdrssh.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/ghqmippcn.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gjbhqcaai.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gqjzzkndk.sHtML


<!-- 参考信息 -->