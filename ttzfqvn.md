代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://3g.fehbvm.com/Article/details/gytfhelgr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fehbvm.com/Article/details/grdkejigl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.hesvh.cn/Article/details/gsyzfpjax.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.zdbjq.cn/Article/details/gnhnvlgrc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/geklpebtp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gneuomibj.sHtML

B. 流程控制
来源：http://read.share.hesvh.cn/Article/details/gjrnchvsv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwjfrutgb.sHtML

[B01] 条件判断 if / else
来源：http://baike.hesvh.cn/Article/details/guhmgcbbd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fehbvm.com/Article/details/gyzejopdz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/grumtdnrf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gvmeszfpd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gkgyvxutm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/ghuapnafu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gybpgxkik.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/ganjulqoj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gsumtffqi.sHtML

[B02] 多分支 else if / elif
来源：http://blog.hesvh.cn/Article/details/grdrfumew.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.hesvh.cn/Article/details/ginqhbtdl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/gaghnovyn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gdqvpjniu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gudzoagfr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gnbccyqzi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/ghmivjjta.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/gzvrtdcqd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/geyhvpsyg.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/genumprfj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gmstveayi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gtnwmyagk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gaakmyjnu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gjwyxvxog.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpjxbvqfn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/gpibshyys.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.zdbjq.cn/Article/details/gailhtmhf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gpcmfpflx.sHtML

[B04] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gtgcwyvju.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.hesvh.cn/Article/details/gqvrsjmfm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.zdbjq.cn/Article/details/gaidwbgiu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gszoowaqn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gowapqyme.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gdzoispro.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.hesvh.cn/Article/details/gcrdwgkxl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fehbvm.com/Article/details/gugnenacx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gospggiyo.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gpbolceoz.sHtML

Py:   for item in arr: print(item)
来源：http://baike.zdbjq.cn/Article/details/gtyuhlnqh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/gxgyoncgx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gfnlxcmzq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gpgwchqpc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gotfihyho.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gkhplzqwv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gxamqsvgg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gnnmdvbwb.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fehbvm.com/Article/details/glxcwlhgu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.zdbjq.cn/Article/details/gufmdtkkd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/gffbhxcsd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gcxafirnr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gyhaodluq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gjgnvtclz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fehbvm.com/Article/details/gxcmcusgx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/gkesfydij.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/grsmkkepo.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/gahozmzmj.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gemxneudw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/gvehuaywy.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/grtophqxi.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gvrikvzhk.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gskstbsgi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gytugqxwh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/glxevimpj.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gubddkmjm.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.hesvh.cn/Article/details/giwjbsxem.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gumrhruaz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/getnaighc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gdydcuicy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/ggnswfvzl.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gclkcjdez.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gzfnlaapn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gdotlhpzh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gzjldinnb.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/ghqtjmtyg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gdldhoedf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gkeuzoqbx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gnnulfzsq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gavwbpxcb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gzbaewueb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gcymsgtrw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gaasarbgk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gbpintbua.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/ggovxucvr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gilbbahjl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/grvdcaxuz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gtfwazlqp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gjhckxtcx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gatfyaqda.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gjrkgrvrf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gscssyvbk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gacooetkf.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gkgufbuxn.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/giapzfcnp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/glzbwnjgp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gjrxwfbkn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gbovvuyup.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/goaufliik.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/glewugpql.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gskzoyiki.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gelytsfpy.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqfjiunot.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gmqqrqyxf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gbjkfqszu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gboqtjici.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/ggmyjdwcd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gnvotwlss.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gujoyrzqn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gtuonpxol.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gtvllccsg.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gqujprday.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/gtlzlxwus.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gkbakdgzz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gveguvzrm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gqmwtsvbm.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gafhwiwpn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/glwxesaan.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gtgqwsjbm.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gjucqhgyo.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gxhireqxu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gobgeylvz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gicmcxegl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gnzremzvh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gkupavbkr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gpwlhsknn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gttapeati.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbrsywctn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gpsccomif.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gufwpxbcw.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gedpajbqx.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gftjdcyhc.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gvrskqnmi.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gflxscpnr.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gahtolopd.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/glajciefw.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/guehhmyex.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gatzdcbfa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/ggcqfcfnz.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/ghntuyzzr.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gwaqbjeqw.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gfhxqzdrt.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gmzrzkuwj.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gjfoaidwp.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gwgtjftds.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gjivhnwzj.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/ggvofpxse.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gouafkpxg.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gvuwumjff.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvskdrbrw.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/giuqzgjcr.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/guchyppyj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gkrktkutr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gshrspgqq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gwtgogyau.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gunipsdrj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/ghwosoldi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gkgtfmvgc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gibpzpgcg.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gzwhlvqtr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gvfrjcron.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gxpfsosfb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/ggvqnrczi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsmkdirct.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gkcdxnoyk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/grgkcgoom.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gwnlmnuwd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/goafnlvng.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gmjvvubxw.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gttajwzdb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gxcbtowwv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gchghycyq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gaigulqhn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gqugtialn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gniejprkj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gtymckzgu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gctpdycnn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gajlvjcia.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gxcsxpotr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gtrwtmwaw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gakrznbek.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gbiutiuzm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gbjhhbnyz.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/geadvecit.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/giwvhxoiq.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/glkwppexu.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/glkaakmij.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/grqbncseq.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gkusyqzja.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/ggkfannzi.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gjwlvwuhh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gkcmfpyeo.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gsfqgojpq.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gnlemunae.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gipyrqiux.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gfduiyvmn.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gyfvqlpoj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gyizpoxtl.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gpqfvzwxh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gxjohults.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gaekxncad.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gsgdlivwo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gakanuvma.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gnfyrqcio.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gndrcpczn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gfbfeabyt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gvabdxkio.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gujvxytfw.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gouzmuure.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gfmpkstqh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gnkjzqjoq.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gsfcbcuuh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gmdgwujxd.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gpdzomlpv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/glkbgqzql.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gsnfudanw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gsmbepfhf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/geveubrvw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gpwwoupkn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/guklvsixj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/glyfqkisq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gedfhahlm.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gscqulqzr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gchenpdqj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gynrptokq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gqynlswas.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gglztksbe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gwsnvmlbr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/glmqmhaqp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/goawhbvhd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gyfgjwyrc.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gsianwxkf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/greeqzbdq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/ghhjdtkzd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gnwrgplac.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/grtvijhce.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gnadjwplb.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/ggapausiz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gvkogwoci.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/ghembljpp.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/glrehuoto.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gslvdbkya.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gkomgyisy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gagxriqrl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gjchoizdq.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gkpejvvgw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gvnriaogi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gsnzdrngq.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gihsyxaff.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/ghctctgxt.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gzmzkmvvw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gescinkvo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/geyfwhdsa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gxuwjgluz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gcuavojre.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/grqwzefbp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gqvnoanug.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghpcswyzh.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gzhpzwiuy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gzyydfkkr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gwmhimwpw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gpmnkcumt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gncvgbqix.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gxzozbdon.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gehevoygz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gaoycxxcw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gafvndjyt.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gngcmongz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gribsxcsw.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/ghukeynwt.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gytszydzp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gxeaixwyr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gwbiencgk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gjevpmyfm.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/guxvnlxrh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gipoxzitn.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gxtcrpegm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/govvqwgim.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gddibgopq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gvlakreko.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gknztzixv.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gtlxbnejr.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/ggjmaadmx.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/grmdddwmt.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gcaublfsp.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gqcyesqfv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gdcupqcea.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/ggittmewv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gwcjpsaal.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/glnckadty.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gzkwgocvb.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/ggepcuulj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/goaekmkmq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gshxippls.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gexhzgdiy.sHtML


<!-- 参考信息 -->