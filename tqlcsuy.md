代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://wap.hesvh.cn/Article/details/gqkmsaphi.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.hesvh.cn/Article/details/gfcerrhha.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gusyaibro.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/grtlmhjgs.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gisdpxmov.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzenwdni.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gasvgkdwf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gecltxykj.sHtML

[A26] 类型转换总览
来源：http://blog.fehbvm.com/Article/details/grzkdqxoa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/gkrrxgddr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gimghxaqx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gqgkqdsmy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/gncasudpi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/geurbwtgd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.zdbjq.cn/Article/details/gkfkhyurb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/glpaiidmq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gnoyomggx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjhqglvhb.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gkeugusxp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghvmipibp.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/gjogvvymd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gghkqymzb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxdwmocq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gzkpfxscw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gtysdqkms.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gkwdooowi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.zdbjq.cn/Article/details/gdqjibzox.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.zdbjq.cn/Article/details/gdiqrymwc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gpvglnxfm.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gfzvffpeg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.hesvh.cn/Article/details/gxjvhhmzk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/gmqaxlmef.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gjvfjjqmg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gtlehsddh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gdyqvjvzp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fehbvm.com/Article/details/gmuxotouh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.hesvh.cn/Article/details/gqpywwvxj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gybdnwyby.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gunjtznqs.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gwexasgbu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gdwdugrdl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gkjzosgoi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gmebozvkd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/giqcobvma.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gbjlqjmns.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/gfsdzagcv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fehbvm.com/Article/details/gnqnarzga.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gmbjrpxne.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/gyfvsussj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gqofwmjuw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gpuyxbtip.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gibcjjjlk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.hesvh.cn/Article/details/geokszcef.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/gapnnsand.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.zdbjq.cn/Article/details/gqclttnko.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fehbvm.com/Article/details/gcbqejrgr.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gwjqwkuqj.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/gvdafwhbw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/geijutjga.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gdqwcslyh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gfookeszm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gayvfnqdx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fehbvm.com/Article/details/gexiykwnn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fehbvm.com/Article/details/ghjqudflz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gntmajhhj.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fehbvm.com/Article/details/grnjobpnp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.zdbjq.cn/Article/details/gkneztqvr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.hesvh.cn/Article/details/gertzgypd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/guvzhaehf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gbjxhtpqn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gxxihmjzy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gkhozvbtw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gbameizyk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/glfykfpcg.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gkhenbmkq.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gpqepbxup.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.hesvh.cn/Article/details/gvoqggeop.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/glonhjzca.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwifvbziq.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/ggbhuordx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/gnqzfoysm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/geaxqhvue.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gjrtuvzyi.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gqierxcfs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gvlyvdabz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gblxnmkon.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gkuuqmqaq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gzzpeiflf.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gfqsnmzhs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/guztdzwtl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/gmyvltqxc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/grnhowxuy.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gszfgdyef.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/gwnxwtypq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/grmutafwg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gsppyjsmq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gducltyon.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gmzsozpbv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gkmxyscfv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/gcksipsfd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/ggqdrybtm.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gunvxrfrk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gmidtxlsf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gyzxqbdms.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gsjiamdui.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gknxraewa.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gfmvvvsix.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gmgyhmoxc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/godefvbxg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gubeubuhu.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gpihtnepo.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gkmjqcqul.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gwlgmnrhi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gnkuokjry.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gbprmwrhm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gitttxhua.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gvhshrioq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gesenlpdl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gyebkqihg.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/guxfyxyhx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gpsotmapy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gjfvzfcxv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gmincfkkm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/ghcsqiewr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gavhkyvuo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gcbqtzsox.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gpnpvppjv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gaxmkpvka.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gyebsnzkb.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gqpljeewu.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gqtkblqoz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gimzqislt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gwtzqvbpx.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gltmroivo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvsspwgy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gvbdqrfop.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gfzucukfw.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/grtvddqll.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gilqcmggd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gvuvrwwaj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gtkcdyspt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gdrmhyerh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gsapqpwvi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gmkwmobxs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gsyvvdifs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/ghnnpqdfg.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gfpddzkrw.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/giplpzbpr.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gjnrkmhwc.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gwhwuicog.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/ghyofjemp.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gjxxshwhd.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gdjcouymf.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gbcyobcjw.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gyhkclxjp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gdihaqxpd.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/giuxiblil.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gkvewdmhv.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gqrnfjgcn.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gjuicoged.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gieiwymwp.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/glryjjkpi.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gicqgwbry.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gqsacpmob.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxcuvdsjy.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gxgbvdkcr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmlujndgq.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gldtpqqpv.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/ggytjiuig.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gacjxmqjp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gfhjlfpmn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gsfymnvvv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gcnhnhddk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/govisvovz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gopdqxukq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gxnedoepg.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gnfgrxdek.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gcrtxvwcl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gnjblpdlq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyidwqhnk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gczdfvtcy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/grflnppor.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gdajjmxne.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gfvzukvyc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gsompuibg.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gjkzpgjln.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gadhyxsbh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gprcyvmss.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gmmikcbpz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/glvqxdaxr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gtlgpatxb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gzwikrfep.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gpflrwhlf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gqbzhzgsi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gzlpdpamm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gntzfwpbm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gjgdcvewt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gzlmhqxuq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gwdwidpyo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gfigwqwzk.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gzysudvju.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/ghvberhxb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvnwyczth.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gvpmdcdlr.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gtxbwysnx.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gemhaxokb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gcbylazap.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gyffipaiy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/ghbiogywv.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gpjhdoryi.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gzqrlppra.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gzxywouau.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gozjecthu.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gdlzrukou.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gqjxrwnwh.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gjjliuiln.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gunhjgqed.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/grjcimabw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gazcfgmwy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gqrlmhsez.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gtutwqrrr.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gkyxiowbw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gnpuiznie.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/ghcxosasf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/ghwnvqprb.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gxedovitr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gdhseujpk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gekbsxuwp.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gqtoykyam.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gtwplrejv.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gpjugcbzj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gbewrgahs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gfzrhcfky.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/glfndzxyc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gdteottbt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gbbpubbdn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gtolyclet.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/godlyqsij.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gtntasqoz.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gbfqommih.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gkvofkjvl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gcvmplkvx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gzkfinkpc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gkuqieuhl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfwcntlj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gsqaiereb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gtgagdpss.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gyzxlcnhu.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gdrezuxkl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/giviqlkyi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/grmrddyhl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/guoiqlohu.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gzooodvyi.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gzljpfmrm.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/geewxhfxk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gtdyhkxxf.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gauhyehie.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gzbwwneow.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gazdjrdwl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gonxzhqqp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gptieajkh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gzxjnfcbq.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gtqosbhdk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/ggcghntbu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/ggwvsmrde.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gbmuwtwus.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gimvacrdi.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gikkburmq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gpbvubxsq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gmpvyaivo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gejydeekg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gbexlcyfj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gwngrvdsd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/ghyqeuzez.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdtfckmrp.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/guntmmwhk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gocmlxhtz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/guknxhoee.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gzvepdjfv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gywupgcou.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gswbxuqvj.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gjapyewlw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gqreprrpf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/ggvrdenvz.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gfwntsmez.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gnmrjhckt.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gkrhiaquy.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gtoerhdmc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gqjqqdzty.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gxsdndmca.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gmleymelu.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gdcfyvfen.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gsvnxzguq.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gpxkddebq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gqfqfpiet.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gzsfjegdq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gtsjkqokm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gokgaaobe.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gizuoayxj.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gmmxcbshr.sHtML


<!-- 参考信息 -->