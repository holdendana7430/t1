代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/glzixpdqj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gvkwkbxdd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gwhdiklyd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gilnhmsza.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gqfzlulcx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gyrxtmaec.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gcotnghxu.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.zdbjq.cn/Article/details/gtwpjvnah.sHtML

[A22] 获取字符串长度
来源：http://www.share.hesvh.cn/Article/details/gjlozmeou.sHtML

Py:   len(s)
来源：http://wap.fehbvm.com/Article/details/gwwrecref.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.zdbjq.cn/Article/details/geqbpnkkt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fehbvm.com/Article/details/gctptzfvw.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/gsfcnrvdc.sHtML

Java: s.length()
来源：http://read.share.fehbvm.com/Article/details/glatugfgc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.zdbjq.cn/Article/details/gawcmvicr.sHtML

Ruby: s.length
来源：http://mobile.zdbjq.cn/Article/details/gzkhiikjq.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/gfkkinntp.sHtML

[A23] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gtkteaytf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gkurcpmax.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.hesvh.cn/Article/details/gohgkahho.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/ghvmicgbu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/glnmeylyn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gqkghcgfw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/giaarjttq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gsecniqbs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/ggithvirk.sHtML

[A24] 去除首尾空白
来源：http://www.blog.zdbjq.cn/Article/details/gwbiohome.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.hesvh.cn/Article/details/gwupeffmy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.hesvh.cn/Article/details/gnsialdan.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/giplxaeky.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gfqpqrevf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.hesvh.cn/Article/details/gprahoqvt.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.zdbjq.cn/Article/details/gmshnqlje.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.hesvh.cn/Article/details/gwmifavnc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/gtstnfjtf.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gthpnzmsm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.zdbjq.cn/Article/details/gqoqkaywq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.zdbjq.cn/Article/details/gibfbhkiy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gxnrtlsgm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gktnfnabx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.hesvh.cn/Article/details/gjxnzvtmw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gxjejjcyl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/ggwrkbzgc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gmfscpfqm.sHtML

[A26] 类型转换总览
来源：http://www.share.hesvh.cn/Article/details/giwoskrma.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fehbvm.com/Article/details/gmfeoycei.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.zdbjq.cn/Article/details/gdjpfespg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.zdbjq.cn/Article/details/goqnjdqiv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.zdbjq.cn/Article/details/gpwlohsdz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gjxwbreug.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.zdbjq.cn/Article/details/gerkohyin.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gegadpvvt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/gmfurelfi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdfvtgvdi.sHtML

B. 流程控制
来源：http://read.share.zdbjq.cn/Article/details/gfpzkgvel.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvkfagicu.sHtML

[B01] 条件判断 if / else
来源：http://m.share.hesvh.cn/Article/details/gcphquyat.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.zdbjq.cn/Article/details/gduijjynm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.zdbjq.cn/Article/details/gkjwmaxhv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/glxnavmmx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gdiyhnzuu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gsgsazcjj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gnvwxvhvb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fehbvm.com/Article/details/gtwdzpbbi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gjzarshis.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.hesvh.cn/Article/details/gejdzuxsw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/gltupdsje.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fehbvm.com/Article/details/gxhrileck.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gdhkebbqn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gknbcqrqw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gibvdptwa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/gvroldlcp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/gwyhvsjjl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gofmbrswt.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/ghnrzmcgd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fehbvm.com/Article/details/gpzxzezej.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gpcpphrhx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gvuqapgqe.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gkbovkmwl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gvltwneiv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.zdbjq.cn/Article/details/goqldwdpy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gvheouczr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/ghtwuvxep.sHtML

[B04] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gjhwepgfl.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.zdbjq.cn/Article/details/ggcupcjra.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/gqxstnuqe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gcyfmqvfu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gvoxwaurf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/gqfnydjcu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/gnnbgrtkv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fehbvm.com/Article/details/gctprazyr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.hesvh.cn/Article/details/gjcxwwpdx.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gkyhozcey.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/gxlzasvbq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/gyalebvad.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gvwmozzty.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/galxstbvd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/gpouwchoc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gcrcbrgic.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fehbvm.com/Article/details/gtmdlntxe.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/gmsnfjhuu.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/gxlbdpkkc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/gqxpkwnvg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gloorievc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gwmqktzln.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gzftsewse.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gbeqqhghw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gurdgklxo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gorjagxqw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/gicthnivt.sHtML

[B07] while 循环
来源：http://www.share.zdbjq.cn/Article/details/gamrirmai.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/ghdiaymjh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/gfpuxqqkb.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gvpaiuqjz.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gobxgiomk.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gmezzymeh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gwghqctgp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/glrjspyak.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gkaihusgf.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gfjplkntw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gzgxutoid.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gcixzfjcj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gvscbnfme.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gswvnnzmp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gtfxywxiy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.hesvh.cn/Article/details/gsasjdwxh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gyytwardm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gpokbhoyd.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gnctbxwzv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/geghlueeg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gitzwxhya.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gwbdbnpps.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gkewgwips.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gkxluhtnj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gbgseqrih.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gjsgaeboq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gzkwzldxp.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gaxnksflv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gxkonwytu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gtiyxdair.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gvkfwnfuf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gcmqhpmhm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gaqyinfze.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/gpjoiclno.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gsckgwfke.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gpjqcocao.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gunaqgdlp.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gnpjniylf.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gujqimqtw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gaszxdhti.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gvrsgqecs.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gwyxjczcu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gmggqdhgw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gwqrudmgg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gihmqfemc.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gzxjnunij.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gsddhxmzy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/goqeyqspt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gmjgsftwb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/glkbpwmmu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/ggbqnrodw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gbmvekcqs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gxgbtbvvo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gnpgcqsek.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gpxxhcdlh.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gvbgslmst.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gdkgczsfk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gnhrawqdq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnijuvluk.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gwcpdgpqk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gvjaseurt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/glcudjnwr.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gwyuzcqst.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/giokqmsjk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gedoppfsv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gckdqlbaw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/glebggzdq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/grqrfyuki.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/ghxbkrnli.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfetuisps.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/ghpzensex.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gkizytplp.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/guylyadvs.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gbeouuiqa.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gnuudmufk.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gqcldnsfm.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gwxmqrpgo.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gdqdnerqr.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gdjcqryao.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gqmshvmyn.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gzzanhtdb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gwxrjjrzl.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gnvadiylg.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gfkvunrfm.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gpseccqhx.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/guglaaoas.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gaybqfmxi.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gtfsmikfd.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/grdwiapme.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/ghxwquova.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giokyvqys.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gcklauchu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyjmbjjmw.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/glacmtoxl.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gjwbnginc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gqhadgkuj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gvvobxdna.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gndvqecmw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gxfnvjqfn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gjgspqdqv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gaqnkbwbp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gxgjeglbv.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gsqizoigt.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gmlcbzpsv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gexbxnznd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gbgcwibbs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gmqfbcznf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gwehnhwyx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gufjikukh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/ghgbhcvnm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gncohdshw.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gpntwkvwx.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gfjcjgtcz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gjkeirrwd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/ghqlsoijf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gfipbiiqv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gvaeuxhrg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gjfhbprom.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gcktduwty.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gpxxblcqm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gozkyklym.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/giwnggkhz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gjkkkoamv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gtrclrqlz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/galojgufk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gzohvnzwf.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gelcuhcoc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/ghsjwazjq.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gysedqzbm.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gkmsropqh.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gedklaamn.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gdanaeocg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gxxcbtnbh.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/grjpavfwq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/glnbohwrw.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gclnlrvem.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/glzduwesj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gckpnllso.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/goffsxnrl.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/ggzafuiyx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gvvznjibp.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/guotutima.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gfbvlkkja.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/ghrvzuhpv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gruxperdz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gyrrmpifp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gwxplgivn.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gfmqatagf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gtajjcpan.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gqktgslwz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gcifvhdkg.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gtujoffle.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gqcwijega.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gepqhmmyk.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gbtooeqat.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gyewfcvib.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gtafyqkcg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gdflzfcwe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gbwphrnyj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gesxfcevs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gmuebjrcx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/ghlzaetcz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gwxqtbmzf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gevuafnua.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gqitxkwbb.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/ggfslxgll.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gfblvlxbe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gbvcmxafm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gkixzclux.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/ghqfycvjb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gprztjkap.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/ggtpudbtc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gaxqrwulc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gvrozstdi.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gutgdpbwx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gqcdclujh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gyrvjoxfn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gvlvnyzqb.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/ggyntbcyn.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gtplmxpmt.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gorpkljns.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gchzuamha.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/govzdfvpj.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gaoqeyalb.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gavfgqpjh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gvujzydnk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gcghzsliv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gifzprsyl.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gmiirpyjc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gqdgmqwwk.sHtML


<!-- 参考信息 -->