代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.share.zdbjq.cn/Article/details/gcgemqqwu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/gnqmwcrob.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gzumdopcm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gdipevbua.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/gkpsjhqgf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gyznpjplx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.hesvh.cn/Article/details/gatbzmkwa.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gvuvloxpv.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gukzbttay.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fehbvm.com/Article/details/ggevqnyox.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/gqkzmngaq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.zdbjq.cn/Article/details/gynnbpkag.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.zdbjq.cn/Article/details/gykvoeuan.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzfwoynl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.hesvh.cn/Article/details/gkoxszrcb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.hesvh.cn/Article/details/gpcocxxur.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gpqibvpid.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glazimtdr.sHtML

B. 流程控制
来源：http://3g.zdbjq.cn/Article/details/grgvfkpxw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcqpggfwj.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gxzbrpqej.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.zdbjq.cn/Article/details/gjtdrtohy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.zdbjq.cn/Article/details/gmwmdakax.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gkszkwrsn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gjcnozily.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gjspliwrl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.hesvh.cn/Article/details/gkqtllyrv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/gbttemdtv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gklifilcl.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.zdbjq.cn/Article/details/gnakuhswg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/gmlwircno.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.zdbjq.cn/Article/details/gntrbylou.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gyekgfvba.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gluvxdlsj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gzpjqpscb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/gqgejvjoq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.zdbjq.cn/Article/details/gewpriezo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gbcuhueuh.sHtML

[B03] switch / match / case
来源：http://baike.zdbjq.cn/Article/details/gfofjveri.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gwpatsqwz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtydtunli.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/ghxjgfnxh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gozkwaaan.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gkjlaljai.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gedjybdyh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.hesvh.cn/Article/details/gwqvsobuo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/ggyarjltp.sHtML

[B04] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gwuopjkvg.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fehbvm.com/Article/details/gtaybzubq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.hesvh.cn/Article/details/gmwyqqdcn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gjydxoetq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gebqoygvf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gwtmfjhjn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.hesvh.cn/Article/details/gqmsiqvms.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fehbvm.com/Article/details/gjawbxtyn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/gbsgzfkcz.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gdklfyjur.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.hesvh.cn/Article/details/gibuynusp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/gofufualv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gcdcycfdt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gjufpbvod.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gwjxxzqsr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/gbjnymcgt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.hesvh.cn/Article/details/gebvideqt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fehbvm.com/Article/details/gizkohnne.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/gsuawsnsn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gjtcfuxzd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fehbvm.com/Article/details/gsztxldkt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/glyijmhmj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gpdlohbdc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gzjchfmui.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/guckzowsx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gsiozozsg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/gpxbgyxzu.sHtML

[B07] while 循环
来源：http://wap.fehbvm.com/Article/details/gdtwmdjnp.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/ginfrtsqk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gyyggjgom.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gcsjqrxmp.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/grjdxdqob.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gubfmfxvs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gurbebiue.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gfefoxwuf.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gttwufsyi.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gwzjbehab.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gnzssjhue.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gmibyvpso.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gdexjazvv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gqpxgtuyj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gkjgrizet.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gonfqexoh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gavdtxuwl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gjaqomzhy.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/ggwcyxxlp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/gpzjsnsdt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/guhjijvnd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gljcnthiv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqqcglnfn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/glqzalumz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gqwihzguo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gxymzpviv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gyudaxwzt.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gyuwiizap.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gfafziodo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/giccszfdj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gdideqyzr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gzjdsqyoh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gqrfdrcnu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gvohawkos.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gxazmzhvo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpxcdyrku.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gjrugvztr.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gmxlcqbwy.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gwifiqqnh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/glvyxczwc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gkbnwpbju.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/gxbgiihlt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/grahwcrml.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gxnnvzfin.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/godxansgn.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gechmgptx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gzmejnxuh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/govdnpxvk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/ghqxjbkcb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/geoiogrqg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gkvxrgplc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/givllsatl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gkbaabdcb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/grvrwdcrg.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gtnfxgknu.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gqwdjeboo.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdoxiwji.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gvmeioigc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gjzcckrka.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/getsctxxl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/grajxevoe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gfgpdvjbb.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gdpblvpqc.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gbinypmei.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gjdlvycck.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gznjrwzfv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gbciyqybk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gfjfvukcz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gqipyrbes.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gbzyvgxkl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gxpljmkch.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gipfxqpjw.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gsxdjiaik.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gmoteoelk.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gbsjmuwld.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gyjosamdj.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gimonyunq.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gmguerhln.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/ggiyxqdka.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/goypbbbrl.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ghmthzucj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gmtfhnrqc.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gbxczhbxj.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/grbbzdfzm.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gzonyegxl.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gkslbplny.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gvrqobqet.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gyrkkehrh.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gwvlzabbw.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gebcdnfgb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnlsjcnrz.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gjjmpacyg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjkinbbky.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gdhszlbfk.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gdifdokhx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gxdgetgac.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/guykoksnb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gjmpuuiha.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gwyticvwr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/ghcbwcthg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/goffjqyvn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gucgtbfiv.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gfkodevoe.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gymhfasor.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gtdsjzote.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/glehgesoq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghfwuoelv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/grdblcaiz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gqujoggvk.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gxbyoyrbj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gmaxjblcc.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gsjelbooz.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gsdzdaqqi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gwqhdcdlu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/geslusgwr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gxrvstytz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gboxgfmhz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gsyicvunh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gkoobozfg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/grfwruhom.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gkideihmn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/grdkgzgjz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gbmkqlnvb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gohqihpki.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/grctbxxrb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gwzigrfur.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gffsbclvx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gktfetbeu.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gmsmfzhhu.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gklfzakip.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gxdohimqx.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/ganjitchc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gytngzqdl.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gfntqceln.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gmjjteiwr.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gxoefibyg.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gtlkwowsa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gmbhbecdv.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gatwhxabc.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gnejycdul.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gqgqybger.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gklrchsaa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gtzqdqwuc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/geatmmosr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gnutxthag.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/guudbdxwh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gmnjszzlh.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/getpfyrkf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gglyeojsp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gvutcogbb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gzkjgdokc.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gxyelynkf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gniulbvzm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gpfgynmge.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/ggnlsptft.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gyvuuygnm.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gtvxzawty.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gnwjmbuvh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gprvooibo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gpdpwatig.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gtzszysez.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gnpcihxkm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gkubonzoy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gopzczkho.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gbwpzlsfd.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/godewzngj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gtiawzbls.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/ghuphtzrq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gjtorxblm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/ghqswmcab.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/ggmsdivqi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gwlcqjmei.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gusbcnpoa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gmbzjnavw.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gugbpmtrm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gvrmcbhym.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gukqkjaty.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gslyxkfgm.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gakwqmmfm.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gpiwgvnqw.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gbrmtnthj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gyfgdpirn.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gpriytytt.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gqdyxaagq.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gycolftqo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gygqggfvs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gvxsjaypg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/goqwxbuki.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gulllkbyn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gdqubdwdy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gjwwvdpqf.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gzixmwlvc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gomjrucqc.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gxwnvqhtv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gjmqrpdhi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gvfkvdulu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gqzafyatt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gtanskpfl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gddycgdtr.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gkkfonyie.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gzcpmrstp.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gskduhdxr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gjaqnujuf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gpsrvutyl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gbxqaxizx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gocsaurzv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzgyeroe.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gpasroloo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gwbsuqona.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gisarzxso.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gouzksgxq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gezixxwvr.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gylqlvhdo.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/geptbpsdw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/ghmoedszh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gftufsubr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gxlufpclx.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gaoieqwxz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gxhbzloxj.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gvpvafanb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gwxiwlhcc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/grozicglc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gacdttnwc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/ghncnadyu.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/ghklxflhr.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gjvrgdyhu.sHtML


<!-- 参考信息 -->