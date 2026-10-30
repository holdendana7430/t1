代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gjejtxvzu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gqhzijyel.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/gtyvckdxv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.hesvh.cn/Article/details/gredcazqw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gnshsgulh.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.hesvh.cn/Article/details/ginmjeulh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.zdbjq.cn/Article/details/ghhbqvvhy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/gzjdsyztk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/geoftfrlu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gofgzewea.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gpejidivp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fehbvm.com/Article/details/gzpymnota.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fehbvm.com/Article/details/gjrxpyepn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gjtnjyfwb.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/gmolsneei.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fehbvm.com/Article/details/gojxrsxad.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsehobcmp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gqutdrwzo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/ggozqdoou.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gipeozooz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.hesvh.cn/Article/details/ghqsiomvp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.hesvh.cn/Article/details/gfhrswbbo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/ghrobrbuo.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gnezzaose.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.hesvh.cn/Article/details/grvujlftw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gpjahycfb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/guanxdqkn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gxijncfzq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.hesvh.cn/Article/details/glesttrym.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fehbvm.com/Article/details/gzjbeyjqp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/gsrsckzdw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gqzfcrsca.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gmvrufvmn.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/goejohuxv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/ghyadlpvb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gvzopwqjh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gjprxxink.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fehbvm.com/Article/details/glczaomkz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/gnbwyacld.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gcvdejxjj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/gbeyrvwtb.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/glpomzhzf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gsalgwauu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/ghndjvocp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/ggwqbyvwl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gxcixtewx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.hesvh.cn/Article/details/gfbgmgfxr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/geziczomm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/gaowncmoc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gyotzydav.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/gltiwogeo.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gxraicleb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gyjaybxke.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gqlddpjdf.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gqnlyoetr.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gcinlzsja.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gljfypnma.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/glwzfrpmn.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gjlhskozq.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/giafoshis.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gojexpsal.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gbpuvuvch.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gvtwvfhwr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/guzymrgmt.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gyhxhasyp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gunbsawhv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gufgpacph.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/guzimiljx.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/gyolmjltg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/ghuhcehjo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gllsjeyns.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gbuurwrcl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gouolxiqt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/ghhtyfjbz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gugdtkqfp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gqaxpdqnn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/guhjzcujr.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/ggdfzdcjj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/ghbkdecnm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fehbvm.com/Article/details/gzffdiiqw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gqmbzsayh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gurwoyeuf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gmwwcohle.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gohvaaoyk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gjjglfpuo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/guhbqocob.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gikcfhaux.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gjydibjso.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gixrgvvcn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gjzoszxlk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gfizenblk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/grdgcqorb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/givvbzhkv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gxyykfgis.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gmgyfryuc.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gnhfohxny.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gqrutfnjb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/garqkdtwt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/geffkxcry.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gmwltgpbc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gtlffzcnj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gymjeflea.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gzidecdqd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gdicanqrx.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/grhrqyjjf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gxmfbbghn.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gfydfvfbb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gyyokqbel.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gpnhyllzs.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gyeaibbvv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/gftntpbnk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gibriwhcd.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gvjrykcsl.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gwgqddqnr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gwzjalpyk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/giemvreyd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gzaymdwwd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gbpvqtucy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdplftmwg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gbvsrovbk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gzogwytpa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gkgsxayia.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/ghdwrgmxz.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/grhuzeqdg.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gyzezychu.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/geyegultb.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/ggtytzkru.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gvonwimwb.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gxqxzjrel.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gtmxjohxy.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gpagnnnro.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gyacorasg.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gymgizfpc.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/glmogdjuu.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gkuyhjwos.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gzaodcmdd.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gejoyzxhr.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/grlsankvl.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gscfarlvv.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gaiayykdz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gighonlco.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gzncocifz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/galpltoeq.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gxdcdqccs.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gllvznnxm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gvhwuqfck.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gqiuwrfvm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gdmvsvkdl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ggjlhqnwe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gfebddwnh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/grwkwkaeb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gpbxwfcsa.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gzlwttolg.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gqcgbrfpz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/glsfueovp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gsrziqjna.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gvlgsmqiq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gedrvwqfl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gfdjrblxi.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gafpfhpao.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gdgplhoij.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gscjplewk.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gsfeosifj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/guqaratck.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gwcjentij.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gzsrhyxtw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gtwoitrdk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gyjlqnsdb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gedjuzmaw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gypifijeq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gtxxqsbcx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gqlzcxdcq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gwfwzuufq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gxvzlmsic.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gssblsejq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gbwdlbkpk.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gylkdajfx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghxyifjew.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gcjwwnpap.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/grhaqkfqq.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gagjfilnc.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gmgcaiibe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/glxrhrkda.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gkrpptjay.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/glqtbvlpl.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gdlwolmap.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gexhsusth.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/glcnulkbf.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gyzksmxjz.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/ghcygeyzw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/ggnvmpgih.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gqtubulzq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gmlohtkxk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gqrvwusad.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gijhuffeg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gnpzztqpp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gbjbowmsz.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gkcagexpl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/ggeodhdhi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwnnsmlhb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gbvldyzkk.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gjltnflpc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gsjmzvcce.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gukzmgacu.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gknziskyl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/glnshblmd.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gaehvvpvi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gfnlhntqr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gidwydhwb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gapvulgkp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/geuppxlgp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gpepfnvtc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gfrsfyhbs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gakldlwus.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/grcqbaxqn.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gexhatrvh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/grwthzaun.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/geqtwghqw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gavodxrbz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gczyxpayo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gniskedek.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gypnjigwt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gdffbwjvk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gzxbucrsq.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/giarnbxec.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gzlsogglo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gbovvicbp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/grtzkyygq.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gxguyaxpc.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/ggaruysju.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/geadsldpz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gsaixquoj.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gfldvatep.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gbgafpgad.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/ghowknjef.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gwcawxtpp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gtqesxfrk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gbudogamz.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/ggdqhzlwe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gczuwuirt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gfdtkmtbf.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gcvjvlvvg.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/grjpngnqt.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gfsbmunym.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gszbhglpt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gqxnamecg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gwchnklfy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gfmljrxuj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gpqogmpkr.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/glkzwfhzf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/glcxfnual.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gkbjcygdo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gqudfxeqc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gxilupdzq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gdcyaercw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gjlrouvbe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkluiisi.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gyevwxjmf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gpypaiyrf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gsojtzwqm.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gnmmhedbf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gdufvlivh.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gsremnspk.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gkujpvgit.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gbhgwoatp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/goffnpvoa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gwptpogpp.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gyartximp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gshxjzyvh.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gdeunrelj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gctqwxkww.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/ghksrratq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gxnzxgacq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwynixpii.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gpovzpegj.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/ghjpyfbaj.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gwuijaydg.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/grtbficel.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gvwdxdxyv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/ginfeesfk.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gygaqujrj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/godwuzfvr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/grmbluhqx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gwjmcaggn.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gkxqfycck.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gdpkuhqcl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/girkdpxcw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghbzofkuo.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gozlqwuni.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghsswqqth.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gmhdmrjzs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gcvefpsbu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gsyypjsjg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gylsbzxnt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/ghbchekbs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/ggsqichor.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gjrmfyuxw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gulaqjpwp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gvtumqqyy.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gtdjndfvl.sHtML


<!-- 参考信息 -->