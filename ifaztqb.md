代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://read.share.fehbvm.com/Article/details/gadzikurn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gbnltugsf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gvmdhwrbu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gkmbanssg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gpazkcmdw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/guvtgzrig.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gmbgqtqfu.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/grejgurct.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gdwjwhqgj.sHtML

Py:   len(s)
来源：http://blog.fehbvm.com/Article/details/gwxczsfls.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/gxefqhlvg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fehbvm.com/Article/details/gdqwuqbpc.sHtML

TS:   s.length
来源：http://wap.fehbvm.com/Article/details/ghltmrwqq.sHtML

Java: s.length()
来源：http://3g.hesvh.cn/Article/details/ggmyimnht.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.hesvh.cn/Article/details/gwdbqsuih.sHtML

Ruby: s.length
来源：http://blog.hesvh.cn/Article/details/gylvttzlu.sHtML

C#:   s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gbqphaspt.sHtML

[A23] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/grykjllyj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.zdbjq.cn/Article/details/gnbrjxldn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.hesvh.cn/Article/details/gpvbginsj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gxyqqsszs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gvdtmelhl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gxyqcsibc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdsgoivsr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.zdbjq.cn/Article/details/ghtoamcxd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.zdbjq.cn/Article/details/gyhyojvyx.sHtML

[A24] 去除首尾空白
来源：http://www.blog.zdbjq.cn/Article/details/gyhbifngw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.zdbjq.cn/Article/details/gamkqjzfx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fehbvm.com/Article/details/gtpvizkkv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gmpookven.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gfkoejhiy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/gfaveyqho.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.zdbjq.cn/Article/details/gizzjdxbw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fehbvm.com/Article/details/gohhimami.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gvtwumjvn.sHtML

[A25] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gvxxmpkvg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/gdwdmnxjx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.hesvh.cn/Article/details/gzcjxwkcm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/ghejzjlxv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gonsphjfo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/glnllelnw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/glkxhfqxz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fehbvm.com/Article/details/gkudpvwrj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gyqhexhtw.sHtML

[A26] 类型转换总览
来源：http://3g.zdbjq.cn/Article/details/gktthkckn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gazhwupkt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.hesvh.cn/Article/details/grmnnxmhx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/gimyqpfbs.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.hesvh.cn/Article/details/gzehrvhzz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gipeegiah.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fehbvm.com/Article/details/gterhbjmm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fehbvm.com/Article/details/gzdoffviq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gxbnakcrc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmuqlqvpv.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/gfxknmprd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geawsptvb.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/gdfyozuss.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/gkbarnhcp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fehbvm.com/Article/details/gmecnqved.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/grtnofqnn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gssbtnzuk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/grgohfvze.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/ghqlqwhqr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/gpcpfsqxn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/goswwrseo.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.zdbjq.cn/Article/details/gkzahulsg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gjzaqwkjk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/gnplrqarp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gygimajwx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/grsxyadkz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gffjpfwfq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fehbvm.com/Article/details/ghtuspfed.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gtufqtert.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gaubzeska.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/gggpywdjs.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/glnntyzle.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gvxocfuje.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gsqlbakkf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gmgxwsbkw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gkhjcygtz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gkjxfbjmk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/gkkwyttkm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gpmgkdbaz.sHtML

[B04] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/giyfcljzf.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/gilungilg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/glgfdpard.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gyjdaprjm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/ghiagolmo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/grfdwjxav.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gstovglwb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.hesvh.cn/Article/details/gothmgqhm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/gcpkdojwq.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/ghurjgmsz.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gxqnhelcu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/guxcxaeja.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gzbtatyvi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gwjsecbwl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/girasqehq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.zdbjq.cn/Article/details/gyuwtzmls.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.zdbjq.cn/Article/details/gioeeiaxd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gnqceprrn.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/gkltovpel.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/gcritnkxe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gxrfvtizs.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gqmnhrhya.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbsuxddox.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/gnvzsoiwm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gmgcrjzge.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.hesvh.cn/Article/details/grhdgltvz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gyuddewsz.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/guorosgmt.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gsxafhnbz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/glleustut.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gnfjxautq.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/grqdmjhzy.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gdunrkhch.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gsvlvftff.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gmaxptogg.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/ghwxhufso.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/ggvlucsgo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/gwtxkmnrh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gtnlcefgw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gflrckhwy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gjnhdyhdc.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gfaoopodk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gvqlqsqtc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.zdbjq.cn/Article/details/glszrccrb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gawmdbbxq.sHtML

[B09] break 与 continue
来源：http://read.share.fehbvm.com/Article/details/gaurtghsk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/guyixwfym.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gcgtipgbe.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gwxokhfwq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gulzkknuh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gsojcazoi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gvqilmvns.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gqcsqjuwp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/ggzkmrkik.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gpcawmdwv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gpjtcqfsx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gaebhxvjr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/ggaznaqzb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gmgmmlkpr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gzcykjior.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gpsktlbcf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/giujimqec.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gcmhrxikx.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/gshfuuybb.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gdhmvutrj.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gvkiavbmu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gkewczunb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gggbngxgi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gfyclcovj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gmdelyqtd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gbutknroj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvjtvdyxv.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gpkohtwxe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gkmmyvfbe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gfhfynsmd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gggxoojte.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gyqyowtrt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gtbioayik.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gkcsddjpv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/gchnseshj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/guuzhbmqs.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/guzjoaqkl.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gmmtuenzq.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkbymfwhf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gqibivdqh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gxfqvdnem.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/ghhlhbpds.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/grgzmwjmu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gpaoqrzet.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gmmdufqad.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gwbbbovhz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gijoafuhq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gpsbgbwch.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gezxlnlna.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gggpblaqm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gswjoalex.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/ggoilloeb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gcyznrmpk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/ggjcqnjeo.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gzahzphvd.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gjjwxyybk.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gzhephook.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/glwasudjv.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gzqystjet.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gfhbodrjm.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/guqentkiz.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gvxqyeeuz.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gkjoxjnrx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gqshrlqpo.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/glglzplym.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/gsrarewxp.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/ghhcpsiio.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/grwlrmfjj.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gjaaiaetl.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gcyrujxaz.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gvlyfgmis.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/goeezgcef.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxjcwssrd.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gdpecdsao.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbtnoxohx.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gdnlrpkai.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gsnrfokaa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gbhnzczsv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gigtjgnen.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqcviotdu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gicqhroiv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gnvtgfgmh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gbefboejz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/glndvlfgq.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gwzyxujnv.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gezaikoqv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gaeyfkzsi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gajkczvki.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ggnfeuuyz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gyqxpvoss.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/ggilnkzet.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gotlkwbby.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/ghhblqkdw.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gogcbexmb.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gklxwboik.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gqhdnfhxm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmuttdssc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gntklmhgo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gybeccjkj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/ghzybjvod.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gwhluxjcy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gkkryifcr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gmaeoswbv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/guqjmjaev.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gptwxsjli.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gslvjnbij.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/ggcprjfvt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gpyhmjtzo.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gtbleuhku.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gpzwgqwar.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gbbbvjmgn.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gensbvzip.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/giwnejvht.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gbobfacke.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gybccbalk.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gsjcuexse.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gsbopgacd.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/ghljobzuz.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/grhrqfskt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gifkdcgnr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gbukpoabg.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/geogqjkhp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gltcjjart.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gtexuitts.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/graqdzquf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gptfmjypq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gmujdmgjl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gfjaxmmer.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gyjbedjvg.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gcigprpgu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gdibojozw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gzejrwiil.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gqzvqdcvu.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gffxwpcqh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gvircteau.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gyadzpwuj.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gentbpfyn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gieghziyt.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gbamrvhke.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gkisttlxg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gctsqmmxb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gcvsgmhnv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gfdsohtua.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gcyrylcer.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gdhfhpvog.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gaiaxqcto.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/ghucaznrw.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gjjghmrmi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gskvdxant.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gdkqdhucq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gzulntjcx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gplleclgz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gilhqaejw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/guwofrhgq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gpqpfdndm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gdzwgljqk.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gceuqtfps.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gnzbblcnh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/geonrfynh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gfsfednwk.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gmlutvpgn.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gnfobmfoc.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gpcfbtzse.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gufuiqisl.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gsgbbvucq.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gxqxvclnz.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gdqxamrdw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gbbjhkjrm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gtcbrgxtg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gfsewnfhk.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gupmrhaln.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/grkuyruic.sHtML


<!-- 参考信息 -->