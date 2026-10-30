代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/goronpzig.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.zdbjq.cn/Article/details/gsxajobxd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gavwfchsa.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/guvxqmnuc.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.hesvh.cn/Article/details/goilnazqj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gfesxqlgz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqyarmmy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gegrmjdog.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.hesvh.cn/Article/details/gakosjxxp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.hesvh.cn/Article/details/gafqmkzyl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.hesvh.cn/Article/details/gtrgyanvz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fehbvm.com/Article/details/grwufaqkq.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gglayhsqp.sHtML

Py:   for item in arr: print(item)
来源：http://wap.zdbjq.cn/Article/details/gmsaichjg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/gocddpvtt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gzptscjop.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gtnmlytsa.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fehbvm.com/Article/details/gslzpavmh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/gisatrolh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/glmmmxksr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/glczfhtkh.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.hesvh.cn/Article/details/gwzbaadlw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gfumqgphb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/gqffygtvr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gbkzvlrce.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gadpmklgc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gnsjnrtkj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/gsxgneyhz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/guudiyall.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/gxnquwban.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/gqgvnpric.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gaoyftgme.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/gsvqbslaw.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gvzuqhnra.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gmravznhq.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gnwtcmkwc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/grmjkedgt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gwmiohfgs.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gkvesihzo.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gizsjrtna.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/gepuztqct.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/gibwdxxsl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gvvsilkeu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gvbwkabtk.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gjbjjsjwu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gukudwgeu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gccffeuxz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gurumqjuh.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gtxiahxvf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/ghezwzjvg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gypirlhxa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gcmxfmrlg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/geusihktp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gznczzhpd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gxzcwriba.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrnyfowa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gvcrxzvpi.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gsevafwrg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.hesvh.cn/Article/details/gyjiukogd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fehbvm.com/Article/details/gnwkhcuaa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gopvckgss.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gwaqiaxge.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gkwuarwru.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/grrdhbhjf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gctgecduq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gpwvlzfzu.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gfkhpycth.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/ggggamain.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gwdpkyipe.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gmbalqnys.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gxbzcxwbt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gkbrdlivx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gdejuuhvm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gztazgdfa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gmihnzvji.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gbcmnyisc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gtrhsjxjy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/ggcvlhjzu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gzefiwkxy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gvnijccln.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gpxiueddm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gafetmqzk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/gbskgftug.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gyeeislvh.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/geeoaearj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gloodixoh.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gvttjdhjd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gjnqrcarz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gyccgwixy.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gdunjiyjh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gepalovcc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/ghjlttehf.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gtzlznvwp.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gudukbaiu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gpjomzrib.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gnuwoydwy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gnxpssyzd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gawqodurh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/ghuvdzfho.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gmivmrouf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gaplhwvap.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gubtqlopk.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gfhnjvjvj.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gocrrtkvu.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gcjbufapx.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gajhehncx.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/grwyaxeys.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gxhiqnzku.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ggknunxmb.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/goduxbiaq.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/giodbbebk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gokrsnfvo.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gtewfpdir.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gwozzfnjk.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gelhjnadt.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/grtamojap.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gyslsyyom.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gtgasrfcu.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gtxkndnrx.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gvwpdsrte.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gohzkizsv.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/ggbnbdind.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giuntgjjh.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gvpkdoclo.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gperziyyx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gmsvgancz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/grvnxytzl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gfjgclasa.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gsmppkiac.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gvmcaugmp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gcprttoag.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gylcvnofa.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gwjuqpwip.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gpbzxmici.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gbqmcpbbd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gegmwnedw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gyseycdyc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/ggwzfehed.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/grwqhqovb.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gnryenfdf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gdavtsqxa.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gkmxzbune.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gfjxvcrxd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gvnzoezgh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gxhlratmy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gqgjvnfrg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gsnpxfupl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gacuyoefx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/grorcxhay.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gmbmoetzj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/guthnkdcw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gsjeeixrp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gycrfhqva.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gucvhgaiv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/guidkuvot.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/grnhvlffa.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfqctshus.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gjlsyghch.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/glxcswcbd.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gxpvvrcoh.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/ggyrkuwfe.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gewvqfibx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gvcckfdhk.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/grsafouho.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gqnklgdfr.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gltwqhqxf.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gzgwzjrdp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gpprofebu.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gdtgocgmz.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gluiijghu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gpmrahqez.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gjgngkodc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gfrrbzwsn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gzawqlshm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gtvcczzgn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gljnnabeg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gnefwjnun.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gjrvswnjm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gsmzjcmct.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/grjgfzlxa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gurybnozl.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gpxunrwma.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gwyzvgouq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gfycfdyqy.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gpsaumzdk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gitwhufxf.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gikwguyyu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gdzvhrtcm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gkpdbnabp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggworakow.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gqrxnvvfr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gpuuxfpex.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gwhiqmpms.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gomfxsndo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gtieqxurf.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gdqnmfcit.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gujxroqwd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/glotyalth.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gtdhrgiys.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gvzxzudae.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gvihwtutd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gkdlttfiv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/glhhmojjd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gxycqgqpk.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gonnnajko.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gacgteqry.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gcwffzuip.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/grkxjrhlg.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gguigowxl.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gamcnqbfu.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gswqryzdn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/goiuiaexc.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gtzkrgozc.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gzzmdyfal.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/ggqelwitz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/ggzslbqsg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gchbzqrdd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/grgthuqzv.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gefmmdgot.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gdaysptxq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gvklegeap.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gvhabcxii.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gytyxavpf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gpzskjtll.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gmrssekpw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gigjfgsqs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gmlvguhpr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gdrdidgdl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gixwfsjql.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gjihuauel.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gdvhzykbn.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gqischgtv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/grsesfvxo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/ggqejicnj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gexrukpwv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gcrfpbjqx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gjxfbyiat.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gppbvkhjj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/goiagmsry.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gsgyqakkc.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gleydlqtw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gsaecvvzm.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gnpwlxdpr.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gcfzqfcor.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gzhpykuyk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gmqtmwyve.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gjfdyfwdf.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/ggujexzhw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/goffihevy.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/grgbflzlu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/grezspxny.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gxpbnvoqg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gpdbvynsz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gesgqawyn.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gahnxcocx.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/ggzrwguxt.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gbeooeygy.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gjykigngt.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gcxfulifo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gspsusrcp.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gkcnwtpqh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/ggcfhmgby.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gxdxctbaw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjzqkqbhz.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gzuqqufal.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/golhpyahm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/ggvvppbii.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gansrtsmq.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gqjssbalc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guaotjzfm.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gmhvurvgf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gpzvznmyh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gzazhikae.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gwplbzreo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gddgiovbd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/guuhgeebz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gbfteycxq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/ginirswph.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gtsgwzrbs.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gnbjdzxhk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gmpbjutog.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gyndlonpu.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/ggpqezuoy.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gjmnozfkt.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gczjvhfcu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqfopvwiu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gaiddwwao.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gkmrtbofx.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gygjcythx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/geaszbqpr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gqadyarac.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gocqyaxiz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gohhnfgpw.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gudakqdwa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gzlewxmuj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gaazvvijz.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/guwkqwqfp.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gmnrjmllm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gcrbtbywy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/glydtcvqh.sHtML


<!-- 参考信息 -->