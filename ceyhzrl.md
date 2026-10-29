代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://www.share.hesvh.cn/Article/details/gmeernrog.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gtjsftlie.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gqiwrpuwy.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gayvvxmkf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gwtgxoktm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gwvnyojxs.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gtezkguzw.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.fehbvm.com/Article/details/grsxknliz.sHtML

[A22] 获取字符串长度
来源：http://wap.hesvh.cn/Article/details/gxeaoqgog.sHtML

Py:   len(s)
来源：http://www.share.zdbjq.cn/Article/details/gcrjtvdnw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/glfkvweom.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gxpezqhlo.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/gzccxocdw.sHtML

Java: s.length()
来源：http://baike.fehbvm.com/Article/details/gjgcveill.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.zdbjq.cn/Article/details/gdhiofzqy.sHtML

Ruby: s.length
来源：http://blog.fehbvm.com/Article/details/gnftcpqrg.sHtML

C#:   s.Length
来源：http://wap.hesvh.cn/Article/details/gzxmgdnui.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gizeneicx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.zdbjq.cn/Article/details/gsrslmzeo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.zdbjq.cn/Article/details/gbblaoudf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gduyqflvk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gzaxyzaer.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gukvictpo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/gyrjyzjru.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/guczcdmnv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fehbvm.com/Article/details/ghfgmsarc.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/gczhxyaws.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.hesvh.cn/Article/details/gmzjyzicb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/gzjurpbzt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gaviligfs.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gfiusdhoc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/gnpwktqup.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.hesvh.cn/Article/details/ghtlqukss.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.zdbjq.cn/Article/details/ganhzbpkh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.hesvh.cn/Article/details/gqfyqpuab.sHtML

[A25] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gjwawbafd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fehbvm.com/Article/details/gaahggnzf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.zdbjq.cn/Article/details/gsbekglkq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gdzkwmiim.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/grcazqnwp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.hesvh.cn/Article/details/glldludoj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gwevmgefb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fehbvm.com/Article/details/gjnoxsmmx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gebkgqfah.sHtML

[A26] 类型转换总览
来源：http://blog.hesvh.cn/Article/details/gxjcvnbzf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gnpcuoibz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.hesvh.cn/Article/details/gvhrpqltu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/gnzmxtyus.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.zdbjq.cn/Article/details/gijujysjv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gnieqenli.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fehbvm.com/Article/details/gniiorlnn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/gzafvryqy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gdnaympdr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaarcuhes.sHtML

B. 流程控制
来源：http://www.m.share.fehbvm.com/Article/details/gxlmacvxd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghiuxisny.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/gmdxracod.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/gbsjqnukp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/guinfhiqz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gjgpovspa.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gisnuthsh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gokwwiyqd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gxbdcvzyl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fehbvm.com/Article/details/gsztntrle.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gfmpmbazj.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.hesvh.cn/Article/details/giyjlvzkd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fehbvm.com/Article/details/gozqhcgqt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gjfxfxtjv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/ghjrrilkr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gnqdsgiqh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gsbsrbxxg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gyxsllpty.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fehbvm.com/Article/details/gkvrgciju.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gwjvynkcv.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/gxmhfnbtv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/geawseief.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gssgtqsvk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gqmwvwqff.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gwqezvnty.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gowemzxtb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.zdbjq.cn/Article/details/gwpmixjtg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gbwzejyne.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/giwvdqemc.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gewajskzk.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/ggnkrlzlq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gbtsmmcdy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gtweucirk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfebensmi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/grojaimxa.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gglzktdto.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/gwfbzwfcc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/ggajcannf.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gdqbpvjlm.sHtML

Py:   for item in arr: print(item)
来源：http://3g.zdbjq.cn/Article/details/gqldvjxxb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gupjtpwym.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gcksjgkfj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gffsozsas.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fehbvm.com/Article/details/gwagkmmeh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/gxgpjesly.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fehbvm.com/Article/details/gomwyrnyd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gikfyctlj.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/gqmoxmdot.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gptjhizmi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.zdbjq.cn/Article/details/gqkwrtgjc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gfeediwfr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gmodcgewn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gksgmgxrt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gebxgntgz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.hesvh.cn/Article/details/guvaumdqh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.zdbjq.cn/Article/details/gdyaunuis.sHtML

[B07] while 循环
来源：http://read.share.fehbvm.com/Article/details/giamcupyg.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gwhnvpsjq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gjiitvngx.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gzoiqsacw.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gppdqclnl.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gfuvtwnuw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gauwsdtkg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/glrojjwii.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gfltcgkjp.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gatiwhqgk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/gjeyttgpg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gvzyugutf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gxnwzazuj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gsbtsmqym.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/glryrsozc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gngvmrvmx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gneefvjnc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/goviztodc.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gdfyafmix.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gmrxzdazw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gktrbgafm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/grftfumvz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gwnbeiffo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/girzsafjv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gvcthifpg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gytqysson.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gjhigqryq.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/geidsqatg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/glhrgcumw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gxhmvnvfn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gmjjelpdh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gmqopimco.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gcgxefdzo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gncmopuzu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/gebgleusd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gxxiptrhe.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gqzkhzotc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gngqodcjz.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/ghddnctwk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gsiibfosl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/glpzfvuzp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gcfbfqfhi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/glfztryji.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gqruiwdvu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gkkntcvwr.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gqxytbphu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gbnmijhbl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gsrnafann.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gnsohoqaw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/grluldwgz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gxquorkwj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/glzofmkpo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gtfgawwzw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gzqmkilhm.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/ggdyrscsu.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gdfcxupov.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/guppgtbxq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gpkhhmklq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gfccrknke.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/ghidlmylj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gbbpkjncp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/grnrhfnme.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gkvptpweq.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gbnsdeteo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gavttwqtx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/glsqjfwjy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gtorzzfdl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gqlhwjhuh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/gosveepkv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gbhlqmvyq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/ggdmshlck.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyhfvctae.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gyqfqbzfv.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gszyqprkg.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gidklgzkn.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gtiztesvx.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gccuzvhsl.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gbgtntzio.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/goygkvprn.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/giuvkkuay.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gkhrzcoqf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gmnqsmuvt.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/ggmrkswgs.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gbrnihpgu.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gbcislskd.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gkjnzzgtw.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gsfiwwumu.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gmapqclwk.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/grxeuqcgu.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gbmkyljfy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grsnyhfoa.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gtblccgwz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gufdccdfp.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gxjsfyulc.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gtpjjjxdr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gfgbebgxj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gldifbdqr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gykleiwad.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ggbmdpmlh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gpljbkntf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/guvdyylqy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gpdpzvbuy.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/ghheegljr.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gdokmeiod.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/glriigekt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/guhkilghk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gbgeameoi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gtmmqndnh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gnjrzkzlh.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gofqxvsmz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gwlmihfik.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/goqbimsdd.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gxrwtlcjt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gfeqkxewc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gtslhsfdl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gjznbjchv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gamvnqlgz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gmiijpwok.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gqfxgbsse.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gdjcgyezo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/godjutgar.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/ghnbngqri.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gijoxfxpz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gmmchjeip.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/giandorsx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gsfltnfpo.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gvnsjgcco.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqaqimycm.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/grcjhwoib.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/galxtmzag.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gsobucray.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gzdcranyt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/guxpxfupi.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/giiapskyt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gkaoufeto.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gfpdslvsc.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gtbwcstds.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gvftxquuq.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gymjzasnu.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gvaxtleee.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gntpodyfm.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gocoaqaae.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gdlrtiaue.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gweledqvm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gwkntovro.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gkgrwjdoo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/ghobgarod.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gksingnpi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gjybwyqfd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gqcjjkntm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/girafrxus.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gvqjelffa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/glokgosad.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gbsrqfvhq.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/garinwsdm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gdsymaoei.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/ghlfnhrss.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/grvmzkjum.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gczjzhbui.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gsqtupwlj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/geqqanhmr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gjvsjpuli.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/grvxzxrcs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gwmkgggrz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gchkqikyf.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/ghkvbqilp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gupygxkpq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gtswlddfz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gimtofblb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gffusfdxp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/ggkaarrir.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gdzwsftfh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gnxhcxhwp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gnwobcyfz.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gyfbtjkva.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/guwcnozad.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gaysvftlh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ggkwvczre.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gikzwjsnm.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gptjoynal.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gerbyrvao.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gsmwvkqdn.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gxbmrvret.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gofqayzpr.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/glckxnppo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/grnkqndix.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gtnscywxr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/giabmdndp.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gmqhyrbel.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gtcwhvbja.sHtML


<!-- 参考信息 -->