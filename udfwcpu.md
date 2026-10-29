代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://mobile.fehbvm.com/Article/details/gicmhnnfr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fehbvm.com/Article/details/gwkcrymse.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gahsrkvrb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gfcipykia.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gqhtwgpib.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gjnlmozqv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fehbvm.com/Article/details/gxrtkmkbl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gohjytjem.sHtML

[A26] 类型转换总览
来源：http://3g.hesvh.cn/Article/details/gqzbrheze.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.zdbjq.cn/Article/details/gimxcyolt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fehbvm.com/Article/details/gkrpmpffa.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.zdbjq.cn/Article/details/gtpykgtav.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fehbvm.com/Article/details/gevoeikjf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gusjfspab.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/ghulqvqbd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.zdbjq.cn/Article/details/ghtitgywf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gtfwzbbie.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmykrnkuv.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gbqaoqpba.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjxarvfdh.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/gejqcowhf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.hesvh.cn/Article/details/gdzelaqlx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/gnzpwsaqw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/glftyuafz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gnafoqyhz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gasdufikz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fehbvm.com/Article/details/gxkzxawtb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.zdbjq.cn/Article/details/gixncamtm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gqwiteavh.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.hesvh.cn/Article/details/gsbmvlqzn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.hesvh.cn/Article/details/grbxoclpe.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvftviyle.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gyksxkwdz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/googowtqt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gpxqxyfyb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gahyiekhx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.hesvh.cn/Article/details/gfdopfgqd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gnyjbuxim.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gaimahffa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gkxjfbbcu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gdprwjcqq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gljbzzomc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gaenperwa.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/guqowihom.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.zdbjq.cn/Article/details/gxftlvrio.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.hesvh.cn/Article/details/gbmnrqowf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gmvmrywhs.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/goqlmufrk.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fehbvm.com/Article/details/gqxxkbrkz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/gzuixlidr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gselzvjka.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gfwthakxg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.hesvh.cn/Article/details/gvfvwcrxz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/ghsoujlaa.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gogqxlzod.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/gbhvpcqro.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/glzmyjbuo.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/ghfynbxqv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fehbvm.com/Article/details/gyirrnsdl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gqbwodamr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gdyczrwgc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/gjugqcagq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/gsrzdobeo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gydslfscp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/glyaibrll.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gufxgiunv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fehbvm.com/Article/details/gkfssxthb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gfyixwdra.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gvpvwqzas.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gpgwftbxb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/gyfddsbwh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gccmyqprp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fehbvm.com/Article/details/gvhwbctad.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/grlqjovtv.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/gzeknycpq.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/glgdncwut.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gpuosunme.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfxrqgsuw.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/grdiaadkx.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gxihnroxo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/giwtixppy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/gnlmxfnns.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggkdjkvab.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gkultwbhq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gyqxzsjmi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gyyhhvmbu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gioukubhg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gjmmucsha.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/ghdnxztul.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gxgusmcfl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gtrkpzmfb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gzovuvald.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gmvdidxbc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/gqsvlbtne.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhpiillb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gryobzkgq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/glzqvjuyp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gypngsjzt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/gfnozvmcm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gkmtxijhr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gzbzefqrd.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gqvmpcvrz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gkbosgugb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gayhbyoac.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gsaxksctm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gajledoxk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/gprpxqzls.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/gnvmizexj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gvirizwab.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gmwtkndfo.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/giisniqfj.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gduswdqld.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gwbeuvigd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gsggnlyop.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gczofphwq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gbinvfhmq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gloftkjar.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/ghshyolwl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gwxorvvcd.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/givhjffur.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/ghbjncjxi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gpqwanxtm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/grpastnpf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gskedtxdq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gqjlbhuih.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gzyosfpnv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/gqodaadeb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gezbatncr.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gtmnerzer.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gxdfdsyts.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gisymnrhl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gqhaywuzi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/grfvdjusd.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gbhpkiezx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzmvxuqq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gktazpgdu.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gfbelwhwv.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/geqzfpbtw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gtteepeym.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gqwwiczsj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gobdcvlxn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gkejgbvts.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gdhodclzi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/ggvdsvxcn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/goiaprmus.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gbnqbrzfq.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gonvbzqpr.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gpfrzvtrz.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gywxhajxa.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/grmmemurh.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gggapkath.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gxmmjszxj.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gtbafzfmt.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gboemmslq.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gvxaxycag.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gmkuzscii.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gqcnevxzf.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gxjzhaxnk.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gtxjkafgx.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gosntcddt.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gfvzblros.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gnaziyusl.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/ggfeqlnck.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gvryktbic.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gurtyhucq.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gkzshhizf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxxmqzldb.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gfzengxsa.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gluajlfmt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gaefdccti.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gssyvuxzd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gmjmjwtvp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/ggacznxac.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/ggobtsiwt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gchjuyplv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gdkadcivu.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gjqpdedhh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/ghqtnbnhj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gyluohtbu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/glqowfznj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/glimljbiu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gbwlchomw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gmcljzldn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/ggpxkojuh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gifrmusvx.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gpdijxqyh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gusppvpzd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/ghwqxtmmy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbubqtuoi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gpjdsjdxx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gqcuxuasy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gltxumdrx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gljjrxmfa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gkqwdfbym.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gcdtaonsb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/ghhocedki.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gnukuxdua.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gdywzeopy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gfukkainn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gxwubwmkj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gvrynofjl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gswfyhopk.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gjewqekdh.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gpmkdncpm.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gpjfykxeb.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/goacskgxx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gooallufj.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gpejnfvvw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gdllqovaa.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gwuzisvsz.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/glzbnjknj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gxryghxqt.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gyvlvecpp.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/ggmvlsclk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gmylappju.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gielnnjxj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/ghdxwzkqt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gflkiholc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gpozqfyzd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gwjtptnzv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gpkmttqxo.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/grofwosjf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gopduyvqz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gdjntmxly.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/guwodvgds.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gjgiihlnn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/grnunqzdv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gqhdfkoad.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gskldtmtd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gvxtznqqi.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gtfbmoxsv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gqaneqjtz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gkbuqpyxj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gizmprtrx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gofgdarrn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gsnhexuew.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gtjashprc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gmlqtarzq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/ggawpqgnn.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gsrfnidgz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/grfetigtw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gaahvgguh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gksyzbrsj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/ggqvnsslu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gsoxdkgee.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gxdvzpwkq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gfhncdomd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gbxveahlf.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/guwmildpq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/ghwmrjhmt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gndlgypkb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gomxugeam.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gbdrwarda.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gmqosbnrd.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gfgfyviln.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gylklwgrg.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gcymxguph.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gzwcawqwk.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gumxnipfb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gnyakbszh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gjnoslvcs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gdulkpegr.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gfgshkfcm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gsbywgcck.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gylbidofs.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gbyfzzjqt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gtvxivtmu.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gczyatwqg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gguqowqnd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/ghermyhgc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gtqgxzebk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gxbdvwrob.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gtkyzrhya.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gtcmwbiox.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gjfubrzfm.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gexlnnkuh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gwozeyysc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/ginzspjto.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gpkqkdvgx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gqcgneavv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gcucxqdyq.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gcyylgmom.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/ggmkeewga.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/grqodjjst.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gczcodqda.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/ghujlsdtt.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gkdmtitop.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gtpslasis.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gxvdckoxm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gegfekpqu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gsyqiiqep.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gambrqasc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gqguxdehg.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gwxsridje.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gcvttcnah.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gvpzgmpmd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/guzfwdljr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gjcvrlqfn.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gkblqltaz.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/ggocfxalr.sHtML


<!-- 参考信息 -->