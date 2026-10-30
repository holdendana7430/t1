代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.hesvh.cn/Article/details/gxzozjtfh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gmjouzlew.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fehbvm.com/Article/details/gibymosol.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gfmibztyv.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gsnoudphw.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnshaxhx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/gtqcoyjfc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gxqtqwxfw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gssgllphx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gcouilmcv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gnvnyjszt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gdpbnaqcl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/guhqkzufy.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gfcatugfn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gyaypcnsn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.zdbjq.cn/Article/details/ggcifnlxo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/ggpjdanxs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/glnmatyjv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gsgnpkyqi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/ghzjppcog.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/gcfftjxyh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/gipwccchj.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/grxpmjvyo.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/gmeltupct.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/grvmowlqq.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/ghnfbbbin.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gtyagepjj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsweetbao.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/glevsanpf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/glujynxmw.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gqyzfglnk.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gcolaeprr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/gzoiuefuw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gttxuiqki.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gmoxyterw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gghnrstnl.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gcapdxntj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gnnaqorsq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gbmlnhqze.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gujuolwgg.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gavqprkvr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/gtiquzktm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gxaikpjgj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gizsmceav.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gmwcukcis.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/ggjcslgjx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gikdkdmsk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/ggihlvwdp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/givqtvibf.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gblnbgkks.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gewstdatx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gmqdpbymt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/grbvyvnjc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gtarupjxr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/goqjgshpu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gqjbjipfa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gutamednx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gqpgfkqlr.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gpamzqcmg.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/glcbmaeuy.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gwwtknarw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gqqzzmzsw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/grltgzhll.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gwvmyoofr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/ggizgxqhc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gftqweyig.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gxgyosxnk.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gzdssspso.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gumplfbsr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gbyrpimhs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gimrypgvb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/grclwqduv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gboidrpbi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/glemdzaza.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/glncwgiip.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gmuskxtbf.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/gdlenflmr.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gesgltber.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/ghpbafmma.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxyaujdgo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gbudplrck.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gkoqdylds.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/ggiekgmeg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gehohwfev.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gxvyjdgji.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gzhslwsve.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gbkpdvuxe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/ggdnuixoc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gbupkshgj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gojlvonoo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gylsqeqel.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/goeioieva.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlqtlpej.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gztuvntnv.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gsvgjqoct.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gawvgqhoz.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gztjvhdkf.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gnobijvdo.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gliiqkywq.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gokimhhlz.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gpbxehsjg.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gfktgjsoh.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gpmbnxffr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gltatmerr.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gcyuzzmyp.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/grhgfrvdc.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gntwpbyeb.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gyvjahmww.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gdimqejsj.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gvqmzmtnh.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gqwkdmdeu.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gzuoktogq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gludrhzki.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/grerexics.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfgidjwci.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gcuonuocm.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gjpsnwaam.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gilozcari.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gzyioupph.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gbbjgjata.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gwozxflgg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gtwaunkfz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gezvxboww.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glkjagytj.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gpdepwcty.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gihfbljhx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gyaxwcwmj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gkmjhhczt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/goksvoztv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/guxpiddcw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/geqjjbzpq.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gjfmgmcsq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gvuoxyuyk.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gelocnanx.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gwlibutit.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gnktptjvh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/ggecdjzru.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gwngirhpb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gapumanjh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gxhqegaea.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gxyklbjft.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/grckjhkum.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/govbzktut.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gpvftbams.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gdcpjpknq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/giqpakbzu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gutajbpli.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gxzyqfopv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/grqdcreis.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gzftctsib.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gvakwldmy.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gfjbbkdgr.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gqbzxvjer.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gcwovmzgg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gopukzarm.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/grdcmlowb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/ggvllvlpi.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gesowzwkk.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gaqhyhjxq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/geawrssyt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gcmubnixl.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gnnyziqvf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gwureyqgv.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gbalcobvi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gyhzbmemb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gdtqlgmmx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/glzmikvbf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gsvitajfw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gjirccvjz.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/goqoqttdu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gcirffdba.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/glrzpoibw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gwfnfhqwk.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gcgbtudne.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/ggjjpidpq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gdqyvrush.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gcgmyyech.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gztweyebx.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gwgbanfyj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gjbgidyjy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gqbmhvusw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/ghzkcnypi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gwseiskfi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gwzaddafn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gvgzkiebg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gqeusihka.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gclftfnxg.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gmoizfyfj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gwymhiehy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gizhekurq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gpmvccdhg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gcucqyfzs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gyexfccuq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gpymblfgx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gmvzvnmqx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gvacmqsbs.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gscmvbong.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gznnlvknz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gogcckgvx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gmoqmguyh.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gsgnlxzrx.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gafhzdfxj.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gmpevebtx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gthwguhti.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gamcbnbmf.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gynznyfkj.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gwglvecjw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gyprhqiqc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/ginswwvry.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gjblevoab.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gbakslhbq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gbuqjjpmv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/ggdkgzmim.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gkudnwwvb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/ggbnnlptz.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gujtjdapy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gjmpjolcl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gnohffayi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gpezqsaqw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/glmlflkqe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/ghxnbguyf.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/geugyilvn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gdxhhhocc.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gnpkluisy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gavuunsms.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gasyfcfuo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gkfjkwdxy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gxbykuzyv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gutewlymr.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gleyekmnt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gwhkmaejq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gofumkmhn.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gghakiaiy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gupermgvu.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gtbethpjr.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gywtrmvkq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gdkwhswbc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/geyfpmgzf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/guzevosjd.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gmaqteagx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gzqpdvijf.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gybckujzi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gickzeevv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gfyyliecg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/grfuxlryr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gayihfjkf.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/ggnygawvt.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gimpfbdms.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gdwhukkcl.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gukvmxghc.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/guswakkgn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gvahkgbvt.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gdxwupktd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gaciivlnt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gtcxikrdy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gjsreqdvu.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gbxtwvniy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/grtyscgjq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gycbwyhpa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyeeyveyi.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gduxxpmqk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpdlunzzx.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gmdkeyays.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gtxthnqul.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gwlvqplxm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/ghziccyze.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gpjtaorun.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/guywksqyu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gopjpameu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gqijsecye.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gfbnainop.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gdtwhppwv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gipoagzxs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gcqqugkna.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gathiprzr.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gzhtpdhsq.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/grbshncbk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gespyfslj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gzfvzvnld.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gkzgjnckx.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gayrsybil.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gmefmpphv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gdrkpzwuy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gmzdiqrbx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gerevpzpx.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gdcicfurb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gdmfhztqx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/ghipzzulv.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gndmhtgzg.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gfhrdfsyr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gvkcmypzj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gjgwnzgtd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gtexafeld.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gpbxbbzjw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gbqbvgqbb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/ggsmqkxzt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gbietmlhq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gbhyzjoli.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gltaydscq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gzehobltb.sHtML


<!-- 参考信息 -->