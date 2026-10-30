代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcrpjdzh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnaxhqhb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjamakfwu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcbdwnhc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnuncbuv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmopbevm.sHtML

B. 流程控制
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuwaiotz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gamqxpuhx.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzygmzpq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyooxfiq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gotvuzglu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gslpeuuwj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrpipxxs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gdtnzppzm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fanxiaobao.xyz/Article/details/grshiuett.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrswxtyh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpigqzeg.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fanxiaobao.xyz/Article/details/gdthskmza.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fanxiaobao.xyz/Article/details/glbdfeabt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpfvyisgb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/gvakcazri.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyajibix.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/glqjqdcoz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjpurypi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fanxiaobao.xyz/Article/details/gumdcwzmw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/gtjuyzwbs.sHtML

[B03] switch / match / case
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmfbyaqo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fanxiaobao.xyz/Article/details/ggagtltfo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtxnragld.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcacrlkzt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gihruxxqo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfvwmxht.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gonejbefl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbkfukdl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftaocysp.sHtML

[B04] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gqincokmk.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/goifmoahq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaafinhn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgtdumex.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gprfkripm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/guwthojqn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fanxiaobao.xyz/Article/details/galaxscgr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkudouhm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gqtmeswvs.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/guicvncml.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeuhrdhr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkbyspkef.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gmmflqzxn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzctkfff.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/glgarepbt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtkmsymp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfrfkovs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnddzmagf.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgmtnwqr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fanxiaobao.xyz/Article/details/grhrbojcc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvlabwud.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gopxfksei.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkhgijrxe.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gxfplpvtx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtxsnjoy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fanxiaobao.xyz/Article/details/gqsirpntd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxhbajsf.sHtML

[B07] while 循环
来源：http://3g.fanxiaobao.xyz/Article/details/gaqmowcxo.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fanxiaobao.xyz/Article/details/gebcykykd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbmtyhqla.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzvrntpky.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtzucuftq.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaxykcon.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gdobeqhvk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fanxiaobao.xyz/Article/details/gbrjgkipu.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslizoeij.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggupaoekm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fanxiaobao.xyz/Article/details/gmheiojkm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxukuvqno.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkrmtkck.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gailxnugz.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/ggizgxdpe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/guxyhqaof.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fanxiaobao.xyz/Article/details/gyxptcnby.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsrjgqbf.sHtML

[B09] break 与 continue
来源：http://m.share.fanxiaobao.xyz/Article/details/guknausnp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjlfmqjx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gojehjgvk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbdqrgop.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtdjxeza.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glxbopxba.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/grxzhskdt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajnrwykf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gejgjtrgl.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gonmogwur.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdfplpqh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerzaptrb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzjqxkuv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/gdmgwawwn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fanxiaobao.xyz/Article/details/glbbsfyre.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkpqzmmh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/glndtbllv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugucjbtc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbsuqebt.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fanxiaobao.xyz/Article/details/gpzfjukhn.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gwygqhhdm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gggmhgzsa.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gpwblxrzd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxvswkem.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fanxiaobao.xyz/Article/details/gossxxrbt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdirrvgzi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjbhazuk.sHtML

[B12] 跳出多层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gogtshkbv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fanxiaobao.xyz/Article/details/gdrfrvqpd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtodnmyyz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgktedjl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gbeaifrcu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gtjoqeyib.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazjdrcym.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fanxiaobao.xyz/Article/details/grwcjvkos.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fanxiaobao.xyz/Article/details/grvrxyzet.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizaybkhw.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fanxiaobao.xyz/Article/details/gjgpxylmm.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/givwszxfg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghviygsol.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gyqaczvji.sHtML

Java: x instanceof Number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsykprmp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fanxiaobao.xyz/Article/details/ghpayhfor.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcpcpylt.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/gypfdeduw.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnbepcit.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fanxiaobao.xyz/Article/details/gbptwgdtb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjmnmaiz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtygefcvs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/glwixqwsu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtmeuumj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgoqhzsw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gfargbavq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfadkysu.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxybvbtgm.sHtML

Py:   a and b or not c
来源：http://3g.fanxiaobao.xyz/Article/details/grebyncvv.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdpwznop.sHtML

JS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gparsocad.sHtML

TS:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/ggejpqriw.sHtML

Java: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsvrqdzk.sHtML

Go:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gtfvngsce.sHtML

Ruby: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gfpxqdljz.sHtML

C#:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsdxjilx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gvnhvubtq.sHtML

Py:   if not data: return
来源：http://read.share.fanxiaobao.xyz/Article/details/gioxqgfab.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giyzahfrj.sHtML

JS:   if (!data) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gqaywftvq.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/grofdmxjj.sHtML

Java: if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gxjmqxyws.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gyglrcurj.sHtML

Ruby: return if data.nil?
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuuqsnin.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrhfwvvt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdcjsspxk.sHtML

C. 函数与作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gavzntosg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gurxjgqol.sHtML

[C01] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeouspvs.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gcnvikaip.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqyemzcng.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gglmxsjmy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gioxwpnnb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjprewmqt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gskfvvldk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fanxiaobao.xyz/Article/details/ggjrysele.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzrdklit.sHtML

[C02] 默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/ghoamuzwp.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwtvckgj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyormcmnl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvxfpivfe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfycttysz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzivdcscg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvypzkcxi.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fanxiaobao.xyz/Article/details/gglpnrrcq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fanxiaobao.xyz/Article/details/ggpzimgkc.sHtML

[C03] 可变参数
来源：http://blog.fanxiaobao.xyz/Article/details/gpxofkxnh.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fanxiaobao.xyz/Article/details/glutjerzd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqofyugxm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvonqskjk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrzdxslx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gywlbvncl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxzwztnk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fanxiaobao.xyz/Article/details/gcvjouyff.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpsgavhi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fanxiaobao.xyz/Article/details/grlfmksbp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gljbswevh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnditedvv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gvadijinc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gxgklfofu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fanxiaobao.xyz/Article/details/gkosmxeui.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fanxiaobao.xyz/Article/details/gkpnvnvsh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoropbua.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtlfdvqyt.sHtML

[C05] 返回多个值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffniiyxx.sHtML

Py:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhvbrdvr.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzfjshwf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/gprreggld.sHtML

TS:   return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaybcacwl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgrfjjxh.sHtML

Go:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtaevvea.sHtML

Ruby: return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnvuyrxm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfhlvicm.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gifxlcumd.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbvjazps.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqquaqypf.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gslwuffvr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeinnrol.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggujbbgic.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofckizup.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gexxbkigu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/glwrkzqoz.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjskfsjus.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbxncyta.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/goxinqldk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzfnnmtg.sHtML

TS:   arr.map(String)
来源：http://3g.fanxiaobao.xyz/Article/details/ggnhmkbke.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gwvpoptqb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaprjmay.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glynxevjd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fanxiaobao.xyz/Article/details/gezwueonq.sHtML

[C08] 闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjlcxpxi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fanxiaobao.xyz/Article/details/gouqbgxev.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxhdfcmq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grocacwdc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdowmsvzo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvkrqkxz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdtdxlrz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzaomoqj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gutsuhszo.sHtML

[C09] 递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gokdjvcuj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfzjjyau.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpgqgulc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/geuhqeggh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gshatnfja.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/gflqrtswx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsqttevr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkcrwdve.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdigbyru.sHtML

[C10] 变量作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gochbamgr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvcanijt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhsngzpb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gyhyqctyt.sHtML

TS:   同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gqmaqryii.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gzggesghg.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvxiinkr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuuwfyda.sHtML

C#:   块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gvmvyzqta.sHtML

[C11] 模块导入与导出
来源：http://baike.fanxiaobao.xyz/Article/details/gqktjlifo.sHtML

Py:   from module import func
来源：http://www.share.fanxiaobao.xyz/Article/details/geyprzptk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fanxiaobao.xyz/Article/details/gbvjbmbcg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcalmhgx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fanxiaobao.xyz/Article/details/ghswyhrik.sHtML

Java: import java.util.List;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqecalui.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fanxiaobao.xyz/Article/details/grwjjapxk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fanxiaobao.xyz/Article/details/gzgruuhzh.sHtML

C#:   using System.Text;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyucnqeub.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbynsuwnm.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgsepfcx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvuezcru.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqrdqysz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhstjsoy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzminduk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fanxiaobao.xyz/Article/details/gqqxsjehf.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fanxiaobao.xyz/Article/details/gieyfyhhi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpohzpzhf.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaxhsmja.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gnkzoyhym.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdmfqdkr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamlwybyy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthdmdqbt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwasifijv.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fanxiaobao.xyz/Article/details/gpskrxutx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrdwzwtw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fanxiaobao.xyz/Article/details/gusgnlbaq.sHtML

[C14] 泛型函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfjfyjzo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fanxiaobao.xyz/Article/details/grzzpzktr.sHtML

PHP:  // 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gjdrhkvnu.sHtML

JS:   // 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gziuqdfgh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwulcjjeh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeeukaai.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fanxiaobao.xyz/Article/details/gmzzlzpjy.sHtML

Ruby: # 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbufzpgf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxzfhwdl.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fanxiaobao.xyz/Article/details/gznarnmxc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fanxiaobao.xyz/Article/details/gpusyiicy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdjuernf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzcaydlnl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmbodksrs.sHtML

Java: // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gieixiwyh.sHtML

Go:   // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gwvemeqce.sHtML

Ruby: a, b = pair
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxsywfvb.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fanxiaobao.xyz/Article/details/ghpxvmtop.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndfvghlr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeapypgt.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqgwwgno.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsnczuvi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fanxiaobao.xyz/Article/details/gwxcbpuwj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gohxcarzh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzaxixqx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grfwyeros.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjjvhsguh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gihrooimz.sHtML


<!-- 参考信息 -->