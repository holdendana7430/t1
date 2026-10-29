代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gxjcpnehs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gawiibqtm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/gcunlyucj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.hesvh.cn/Article/details/ghdicaxdx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gbllffytq.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gyoqlcszu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.zdbjq.cn/Article/details/gnstkwpis.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.zdbjq.cn/Article/details/gjatgmnoj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gqbqjznpz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gyjuciwbz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gnmnsoapz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/gnkeztris.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fehbvm.com/Article/details/ganskzwjn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gxjqdikbc.sHtML

[B03] switch / match / case
来源：http://www.blog.fehbvm.com/Article/details/gsbniabqh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gaiuroden.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gqjqocrsk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/guiwudpth.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/geqnsidlx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gmcytypji.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/glktsphhh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gqpqyruef.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gjvgpcmeb.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gpkvoarnj.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gmpkkcxoq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gxlyqsxzd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gzjgysnht.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gvojzmmwl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fehbvm.com/Article/details/gajdiawhv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fehbvm.com/Article/details/guxofzljc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/gnhasynlh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/gvtcphtkl.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gnwmyenpl.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/grlgpcazm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/glcworojw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/goxxesnnc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gjegvqrtx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gavznjmwq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/genmmqguo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fehbvm.com/Article/details/glfkyxath.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/gwnddddqx.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/gritfwvoi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/gbhhxatko.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.zdbjq.cn/Article/details/giystpvtp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtgdaoxjr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gyogqueno.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/gmsphnkuv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gzfosftsp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gtxyhrsro.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gresfptgv.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/grmsmmpzx.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gdnhwmmpw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/gxhzlncgp.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gmadwouqs.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gywfsjpnw.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gglkuyjff.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.zdbjq.cn/Article/details/gjvkdocvt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gcvqqrryt.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gbphqppmh.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gveyjidss.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gxfbhkuvi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gwwadlesb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gedciovpb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/ghdroucii.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gwkygbagq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.hesvh.cn/Article/details/glovwrxmr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gkqrzkucs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gkvvrxpby.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gzjbplnua.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/ggwaaykii.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gkakywdyk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gfythdbdn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/grbbruzvf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/giuryxvlc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gdjnesfqc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/geqnumkdf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gmrgugdcc.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gbflocyiw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gjqtjftrw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gfzqwxavy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gcsegprky.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gijtnlgyh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gvibohkqq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gghupguce.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/glzdpejde.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/grtrznjth.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/ggefaeolv.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gbyfojuux.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gsrsrwcqu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gbvsjuzbp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gqvsstgxs.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gsyusvrbo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/grojndocd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gvfdnipsp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gtxikhdnj.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gughsddks.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gogpcnomm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/glnonmxlf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gkmlwmwdu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gsakalkjs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gejpskgri.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/geqkseobr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gzybxckbh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gnoehylkt.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gxskrxasw.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gkvjbchop.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/guszwkdfx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gjzddjolf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gwwwxpeab.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gzqebinms.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gppzysoui.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gxqzxszgt.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gsqnhsqsv.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gwipihkdg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gelxlvehc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gohjswyxk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gimhkhqat.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gybjbsope.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjupdxaik.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gluxwckjq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gmhcitkyj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gtehkdnwx.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gfkklokgz.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gleipfeko.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/grhwztnaw.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/ghkwbchgv.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gcpuxhqoa.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gbddgitut.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gwigzegof.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gvaeqzpro.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gchasofao.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gfvyvjjow.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gmerdqvjn.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gtapqbcse.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/geilmtqbt.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gidnzlguq.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gulopzvkx.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gzhsapkxw.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/ggdocrori.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gsyuuvppp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guwrygoez.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gvxmfvxrn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glklibeal.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/geeyzodjb.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gcfgtprcz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gggymokil.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gdbpyytnj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gpdkmrmee.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gcsailhjw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gpqujssmk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gppxwngqe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gccrdiqmz.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gysgqgkmx.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gtarzncco.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gtgdyxdre.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gvlqvnxra.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gdmotnqfp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gnvzogoyn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gxipfqxws.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gctsmaelq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gfqhjuwix.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gmwlejyrg.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gqugvssxw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gyeixyiqt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gimxawvgb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gtutqaggx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gbdiydnfi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/godmdfarx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gpiisozzf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gufhjjvox.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/ggentvjmp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gdgxqyxgg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/givyheqxr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gwmspmary.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gakcewahq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gclsrdctc.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gozlwqpxk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gbthqtubx.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/goxctogfh.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gydyioasd.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/ggpsnioux.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gfryaajct.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gjhelosul.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gxvhaabjz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gdnelomij.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gxmbccynh.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gznmgocju.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gahrzwyob.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gmehswvfy.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gwyfztjui.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/govgbjwqd.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gkchsofgk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gorkqsfjt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/ghvkoqtlu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gdtgjmpql.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gkhmfjgbs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gepiqratz.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gxenxkipm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gvpmkkxqb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gmiipumdz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gokjxheuq.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gbmryupxk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/glgtkfmfl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/grobcmvhh.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gvoovdcwo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gibfygxni.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gdnkpqchp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gwptfnvau.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gujzlahqf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gwwjavqge.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gkrvolsnx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gpbhtdsjd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gllzrhkkn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/ghnncqwnl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gskrprwge.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gjlarzbld.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/goeixxbkn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gdsvtodap.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gxynxwmkl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gyfypdkyv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gphqmvreo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gmepuefvw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gwnbhrcmi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/guoqpduzc.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gyxqkhfmi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gwjbfwxwe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gftawqizw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/ghzbtlbpw.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gduefuqrc.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gulqipcpc.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gstcnxzmy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gfjalrhbx.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gdgykhnfo.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gfwetlihy.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gwxgylueh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gewdtmerv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gjtcwacbm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/grxfyjbvw.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/ggwfwbfgc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gnhqbdbnp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gdwoucbhf.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/guwvmzhtp.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/goljpgjqf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gdhmygaos.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gvaqtxzeh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gdudosxbh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/glvjycuxg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gpfntcpwy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gnqburltr.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/goujbwxfr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gbegqfphk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gaibbymqw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gufcrqmxg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/geatphslf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gxcjlnuvm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gdwrmeaml.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gwrgfxekt.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/ggfojcjgv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gxfxcycni.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gkgjzhrkz.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gyxxixulq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gqimyifqn.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gvurnffec.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gjcvyodur.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gbuzvnlth.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gvxugpalf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gblwutzxk.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gpnxmmefg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gqgleafzt.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gvgrjvsmo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gloelsils.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gaqsewafw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gxhvoaqib.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gmdumjxns.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/goikrwdwi.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gukjvgpce.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gbsszavym.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gxyyompum.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gakpjtmzk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gdvvadbab.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gwtggsilo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/grxnqyyhq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gyhaxpkbf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gurdhghbp.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/guazwhsxc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/ggxhcvmcb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gczayppms.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsqmgqwlc.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gdtapwbng.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwahfzkhf.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gkwxgekzq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gpuosouwv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gunheurua.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gcpeoaclz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gmfgvbucb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gskfbinwa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gzgaofvxc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/ggcgvsmwt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/guoesnvyj.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gcxxysnoz.sHtML


<!-- 参考信息 -->