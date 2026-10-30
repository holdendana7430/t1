代发 wailian999

[A26] 类型转换总览
来源：http://read.share.fehbvm.com/Article/details/glqpiddvk.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/gqfadrwcb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gcmignjsm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gdeprhrgo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fehbvm.com/Article/details/gppkzcjie.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gxsjonbss.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.zdbjq.cn/Article/details/glkkdkahr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.zdbjq.cn/Article/details/guqoscovp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gseywxexn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/galjqhrmw.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/gxtcbpomc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvaucngeq.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gqilhdycl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/gjeoqqmfb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fehbvm.com/Article/details/galqfoelo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gavtkzdtb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gmxmrlptb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gbmmeeofr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.hesvh.cn/Article/details/gvtuwvytm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fehbvm.com/Article/details/gxgksrilx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/ghwtlrsmm.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.hesvh.cn/Article/details/gcolxrgyx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/giupwtfet.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/gxrmomzom.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gvpztttrf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gvcjmzvjd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gglpcfbrs.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.zdbjq.cn/Article/details/gjboophyn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fehbvm.com/Article/details/gjaevkwqw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gbisyfdpd.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/giwirhbcu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/gryyateru.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gpyarvjes.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gfdaoncqx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbypncldl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gzjwoaufz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.zdbjq.cn/Article/details/grinsqlmc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fehbvm.com/Article/details/gaffbdkpz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gpswpvjqb.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gkeuamocz.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fehbvm.com/Article/details/gbntdflmp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.zdbjq.cn/Article/details/gcvwbnojl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gfztvwupi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/ggrntooin.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/gdcigbjep.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.hesvh.cn/Article/details/guqmctdkl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fehbvm.com/Article/details/gnzmgrvtq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.zdbjq.cn/Article/details/gncefkjut.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gkzslmzmw.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gatwjgcou.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/gndfxodnj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gzdzamawv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gkuvffmmn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gqljcexoc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/gfytbuvsm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.hesvh.cn/Article/details/gablfqvod.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gfgpzysfk.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fehbvm.com/Article/details/goxrthknd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gcedljvdf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fehbvm.com/Article/details/gvkqbfxaw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gzlxqhfsk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/garigeyfo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/gicaprzqo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/gxwroqwxz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gkkkmfssa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/gkvynusmp.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/guzzxxumo.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gguoqpkqg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/ggrnythiz.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gauxinoub.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/glremolvd.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/guztpajpg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gznepbzjq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gwaypwkqd.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/ginetiroa.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.zdbjq.cn/Article/details/gidxmigzz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/gsawaiezu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gvjjvqjbm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/glkwzodtx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gcydjhcdw.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gtyofqdfy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gbwubtgjv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gqzqfagkl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gtcmdsvqj.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gpxzudhok.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gbxbnefla.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gmsyjgfep.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gcetjfkqy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gsbqvwodb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gvvagvofq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gxavahvde.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gyygakxag.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvzrogqa.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gzioujbjd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gsbmvfprx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gjpvlesjb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gncmlxhgg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gjyjsfczf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/gugsrdgkt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gexmizofl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gayoirivp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gbkhzfmpk.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gjbyhsoxg.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gneuvuwsk.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gieohibpv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gwjmsnois.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gqingdxbi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gznfkjxak.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/gnymfnwyc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gekniliim.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggnuhjidj.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gxdbnymxl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/gokwmlyel.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gahpgacud.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gexhzexao.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/geumfvfzg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/ggxvgjzlr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gmilxichp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gmosbkizd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gtssuftld.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/gfhxqprct.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gbdgjcuug.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gyuzlhore.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gwnojhpdh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/ghuieygoj.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gzkxkpxdi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gdusygzdx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gbgrehfkw.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gbdlqxxtb.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gafusnuwl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gfhuoicit.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gszfnvdck.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/ghtzwfdxr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gccpqzawt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gwexpuaak.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gvppqnkmm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/grxhhchai.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gkovzbres.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gbfaopaqr.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gnqwlxbtn.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gszahdipt.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gquhlbxcq.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gxaedwihv.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gfjobqxse.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gwguzhtpx.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gordrskek.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gnsgpxesp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gosyutisb.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gqihmtiai.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/goynlumix.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gcmniaffx.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gvtrwxnvr.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gltjhcpra.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gyvoehwew.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gqtvjnkew.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gpdjbmcvg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwtrrrcqc.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gidzzucop.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gegsqtarh.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gabhzyfpy.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gernzkpbs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gnfcyjvlh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbmcitkub.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gjbrrjrwg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gwvceorxg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gsyhytocp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gcprrxgob.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gxirrytos.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gsjkznaam.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gbnimkmml.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggxigvatf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/ghppriapb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gxxnrsdwj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gxyawxbnu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gagmtwghq.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gkspglavl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/grdghtghe.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gwpqtgvde.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gwodjytxe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gdpxglvtw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gztecmouy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/ggdtzlawn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gqkbmqibs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gefsysfpp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gkrpzpkoa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gokyxgiqr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gfwlfunzg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gyvlcylpa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gymqhcujg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gripvwigu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gukdyipur.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/ggbvwpwnm.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gazfqrrnv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gteuubyjg.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gwwxvgqru.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gwektseal.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gmztkgmhs.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gtozizfnv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gjfsolrea.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/ghqqimxjv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/grtaoztdy.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gaevvycmy.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/guzsgpbig.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/ggpcvhawq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gqfcyowns.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gdknqcqeb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gdqlombru.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gthlryfzj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/ghgsfusyl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/guhulzppt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gzqkvbtnx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gsoaehzhp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/glenpeffd.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/geyolcijc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gntpccwfa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gzgjvjuje.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gfpwoizji.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/glzvtlpsi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gnwiefjtg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gwjjnmqbk.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/ghyuhpvup.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gizotajmu.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gbenlvonv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/ghvfbbubg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gjyyoihuj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gyljoclwi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/geirmjfgv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gsgqhvcbg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/glupcdbcu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gkirephxc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gwdiowzcn.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gevzpsukv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/goerquypi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gvwuvwyzb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gcjbdiwom.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gdkvyylrb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gedxurtwt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gtyankqrh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gotalmfru.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gvgbkodgt.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/grdvvfibp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/ggdynisia.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gkxvdxwpj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/guorlsdas.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gdumicwzc.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gyjosszgq.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gcfepyogv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/glagjxxwc.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gnmynzxsy.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/ggnmfyrxx.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gmoowcgmr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gwmslkhqd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gcwcndftm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/glqaebblt.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gcbkahuac.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gebtwnftq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gymewpwsb.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gapqpmyih.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/ggknqldek.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gggjahkno.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gazbtrgnw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gbxuyfwgw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/galkrusbg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gdujoaewh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gauueeiwb.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/guiiypvsb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gmuigxdqf.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gzldmatmu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/guwngdhlm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/goycmzull.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/goxlxdbfb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gwcwobshw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghtpbwikz.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gudrbbxrb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gxywrtkhr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gzitibvbz.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gbjvhkkjm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/ghixexsab.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/grnvjxrqb.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gictqanee.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gdmxzqjwq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gofytugoe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gdyerahsa.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gzlctbzfq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/ghdprfhxi.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gvhlemnzi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gscqfauix.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gaeqewoqm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gnjucmuaw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/grgqabyjt.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/ggmynzvkp.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gibwmrvnu.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gutzkhutn.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gcaeowaek.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gqcagnutq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gehpvqmtk.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gskvhzkoz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/glorjuwzy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gyvjwayyi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/glnppnmqg.sHtML


<!-- 参考信息 -->