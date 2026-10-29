代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvxusvun.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fehbvm.com/Article/details/ggbzsyrah.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fehbvm.com/Article/details/gocuyujvg.sHtML

[A25] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gkmkoxhnb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.hesvh.cn/Article/details/gnuaqrxxn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gpbidmsyc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gyyxqgsbz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/getjzsvca.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fehbvm.com/Article/details/gilkhohmz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gptsaddfs.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/ggrojkeem.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.hesvh.cn/Article/details/gimyxxilp.sHtML

[A26] 类型转换总览
来源：http://mobile.zdbjq.cn/Article/details/ggafyhpye.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fehbvm.com/Article/details/gjuxlhhqx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/gunnwqvnc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.hesvh.cn/Article/details/gciudiepo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/ghnxfqohq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gdnkbqama.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fehbvm.com/Article/details/guppdesby.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.zdbjq.cn/Article/details/gomoopffb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gcpqjduql.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guuynlcgn.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/gxnnunlxm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxwynnkxm.sHtML

[B01] 条件判断 if / else
来源：http://baike.zdbjq.cn/Article/details/gdyigwvzg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gwaldvian.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gvjpucthh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gwawdujai.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gbpfgmimq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gysgjtrzp.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.zdbjq.cn/Article/details/gwdvukqpn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gfhnxtuoe.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gbapqdexg.sHtML

[B02] 多分支 else if / elif
来源：http://baike.hesvh.cn/Article/details/gyiwxgeev.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.zdbjq.cn/Article/details/ghxgbbcif.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnfmiuapm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gofiolzge.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gcpmlnvgd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gfpyzksds.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/giyvxsokc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/gjcdqfhnb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gduexakjp.sHtML

[B03] switch / match / case
来源：http://www.share.zdbjq.cn/Article/details/gosrkezev.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.zdbjq.cn/Article/details/gmjzdtasp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gszwfriku.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gnftizwir.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfkrayref.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/goyaoqxyt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gmoljepal.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gtgajcgqq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fehbvm.com/Article/details/gwjdczzma.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/grezcorvf.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.hesvh.cn/Article/details/gijfczzlu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/gdoyvikoo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gnazhsqjc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gbzwepzvn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/gbfumgnrp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/grzgoxnmn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/grpseytoi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.zdbjq.cn/Article/details/goymglpul.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gxunyuuvv.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/gcwefivuk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gscivjqyv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gspdzsjed.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/giosywbhk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/guyrigfxh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/grnkzjfuj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gyuistqtw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fehbvm.com/Article/details/gvzgqhnya.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/grxhjnpeq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.hesvh.cn/Article/details/gyrjbdhuo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/gnwbinfgk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gmjiazzdm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gehcirotr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gbrinkynk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/gjtlblvkb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/ghqhnmjst.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.zdbjq.cn/Article/details/ggrqgdxwb.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/gzgsyjumt.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/grssryvws.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gaxydfjrk.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/ghgykniqx.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/geessruhl.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gnhxuoesk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gjtkoetli.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gjwzctibu.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gjgjwnbpy.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/guuvdzgym.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gxasapgat.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/gvgxjwjpa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gqqfowdne.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gnjnhpdhs.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gomhomher.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/grdonitee.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gqtbvkhbo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/ghexahmdq.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/ggmgmaogx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/gfpdxysfv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gfdnlkjou.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gyjobeilb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gzrfodjqq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/giqecwmdl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/ggyzqgmxs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gciviooya.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/glohbdggn.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/geypqqfsd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gtglfpiyf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gyjxgmrpu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gidxrpgly.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gkhovdztw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/giullkzfg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gyqwnyzcl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gbtgvxokc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gekiyiztj.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gqthdonab.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gzklnjvmf.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/garupafoc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gwllgazut.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gyhazyfha.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gtwxgyloz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gdzbgzifv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gfcrnleyo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gvoqsqiok.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gigunkxfx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gineodbrm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/grigdjmte.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/glrrixtzb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gynpmphhf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gmvfcbyvb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gnwcnltug.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gtvyublzd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gvuzknqqq.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/givuoowlk.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gxdrbwdxh.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gutjzmwtx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/ghdkyfqqr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/ggyusslox.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gbuigmgyg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gjcbzcodz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcvcxnzs.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gnehdiyai.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gzzukimby.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gqnyenmjh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gnprtbfqi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gkwojnqhg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdymonwsh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gufpzrdfo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gldtnomme.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gnoehrnkd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gqetixoov.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gbbyumuqe.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gbqusszxt.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gljmbjyna.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gnbhvercs.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gehmxrhtj.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gfkcysqny.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gplbovjwn.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gowcbjsml.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ggzhpplsw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gehqkrewt.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/ggtckyqdt.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gbvdsoufb.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gajjsyvpo.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/glmxthpni.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gttysfjoo.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gtrhhupjy.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/glsllycsd.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/ghaapjkzs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giuwokpvj.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gappshnhq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grwzptmhu.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gofdgzggh.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gydmtrxbp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/ghdbivlyt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gkqvrrtcb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtyizaio.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/ggagdxwaq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gfqzqicxv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/grqjebppc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/glikofhnb.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gqvdxlalx.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/ghsbzeret.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gyomqhasl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gfvxikirs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/grckpcirq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gafamfmgl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gweabqtzh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/ghilzjieh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/ggrrcktna.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gshoqyykq.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/geuzdaaqs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gvkfnlzpm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gvwvpqdad.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gbmujebsh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gqehhxiqo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gnxzunwkz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/ghvmzywuq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gtqkwyhwd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gqazmgvbh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gssvvqgts.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gzzkaiiyu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gbrabbjie.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gdjchggyn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gpmzxzmxh.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gnlqdsivl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gulfbinep.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/ghdvavcpk.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gfawoekox.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gnkucdosx.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gyzeuuaos.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gqzkahwai.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gmfpmerba.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gditogexy.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gnadxtwrg.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gpclkukvq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gezcvxkos.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gyloxdyuo.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/ggfnqmzvn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gjyywyxxb.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gldxpnfof.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gyadwdcha.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gduqlbojn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gxquyddpp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/grzlkajdg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/ghaskcedg.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gbepyedhu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gntotaatg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gqyfueyhv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/ghqjdsqbr.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gbkmjmpfy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gvbojqmlu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gerzmsehm.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/galjlsamh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gyirkjlmg.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gzxgbjemb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gqmxlssbb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gvdhbujev.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gknxcemwx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gylvicxjz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/glxibgmsq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gnudpzdle.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gkjdnblcs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gjouawngc.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gvaownrha.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gotsdtnpf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gkwweluwn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/giibfrxsm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gxwbpvyck.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/ggvovsiia.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/grfhjsevx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gkrmzwuxs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gzefptnar.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gkvpmkfhp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gcifwvpxf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/ggnoodvjl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gjhyeupty.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gvdzytuxu.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gpdyvsbrx.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gejycwxkf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gfwyljkxn.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gvplphaiw.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gddoucxel.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gwbwqmsso.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gismjgbkz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/ggulhvutq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gfkxnfzhr.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gyhuhuzzo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gxhxmpysr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/ghljodgdn.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gomndtmfo.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gpokqpmax.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gfqrthmfd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gzwdxxyus.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gmxwywwvt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gedxgzikg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/getclkgnw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gugirkpmh.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gptocpezv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/giardbsaw.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gghrpuavr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/ghnpkhfex.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gtpjcovvo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gfhbsqnme.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gulpdaifw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gmtyioerg.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gpuyzmqwr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gleemdebt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gknglmqqq.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gvdzfnnae.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gcfuzgacz.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/ghondskjf.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/ggtnqgnxj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gvzjzskqw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gfnryulgo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/garftonma.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/ggpcecxfz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gppamdugl.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/grwxxlduo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gbyqdjyri.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gpcuwuhkd.sHtML


<!-- 参考信息 -->