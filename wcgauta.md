代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fehbvm.com/Article/details/gtrvybxqi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/gyukjsneg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gtqgxigcc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvwsrwmsj.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gcrdojgme.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/gkysldqfq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/gmaimzgik.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gntuxdgng.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/goavjrrca.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gykfyqqkg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gqgeifdff.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/gjavijdms.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gnixxwkxa.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gpzzbpuup.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/glfhpzlru.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/gvuxjyjrm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcenuvyxe.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/ggyqardht.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/gfeszibfn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/grawnqjej.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gcjdutnfx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gifzfhcgm.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gqqnbntri.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/gcokunfei.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gbpzeauoa.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/grforkanz.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gnyizkxft.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/godzeivqq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gvjmiwryi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/geehcoryj.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gvbdcbfix.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gshajwvxf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/gnwlbbeek.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/gqjzjpphs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gnmoqidcf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gousigdos.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gjcrtwnsj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gqiqrtuho.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gnokgupqk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gchuhtcyu.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gcdeaaakb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/ghzpenoqt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/grnmibpuq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gagtyhurv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gewltgymh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gclwfzvra.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gkwvdtbtg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/grodqctgk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghelkgman.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gmprfghic.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gnhdlilgd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/giobnkrpu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/grzsfpkex.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gllrqnvkc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/ggrkikjkx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/ggxcyqxir.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gjmibgqcu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/gzfxyoamq.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gpscmtgip.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gdvnbmwst.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gciqdgmva.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvbcrnvea.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkfxbuicl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/ggzprboip.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gjrydjrqg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gdbjwblmc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsxjkavm.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gsphcjkpw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gwvdjaate.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gxcwbupcm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzhzzxdp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmuzjhus.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/ggwacothq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gdizdtryw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gsrvfxgxm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gvconcbhh.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gydhxjuyd.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gezdkfgxh.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gzvlptiiy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gjebwuzwm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gzmdqqpxf.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gzzqcbrrc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gjqcwlkga.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gfpsfoadp.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gtgicstza.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gqmvsoxjc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/ghwwirknu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gxzujnmtl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gszvvhtiu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/geqbuxwkl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gnnjjropw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gkcsyhwnb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/ghwgnuzpw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gttgeikrw.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/ggwkgfbha.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gvydxnvxs.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/goxryqknh.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gksjjyclu.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/grglhpnbp.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ghnqgfwku.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/grmxjspfq.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gwgnpykbg.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gajjsiplb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gtxgprkhb.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gseafexxe.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gxvhiwxls.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gcfrpmofw.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/ghyplpuvr.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gfpwuitux.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gqngualgy.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gsuwpoyxr.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gpqcbymyw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzbdwsdwz.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/goxghuhoa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdmhfagaq.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gfmnuesbu.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gcpjzsdkf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gmosmcscg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqxlsmrrb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gxgvsanrr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/grtnebrwz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gdbmkyazn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gztreeosz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gatwcycim.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gltodzeds.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gzlllnady.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gdiselyht.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gsjqntuix.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gqymvbuxs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gmlrfkkmt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gxsemrkfa.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/geqkpbsfl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gzcedmyyn.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gmhmfquow.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gadrwxrcr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/goderxqrr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gmlgikzva.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gyxsfrrvp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/grqiotopj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gsfwryjac.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/goooypcok.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gatoppwek.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gzszktjim.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gupxifleo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/guhxcgjwh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/getkkglga.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gueogfhmp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gltldcvai.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gvrscvbyc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gndwcrumx.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gblftsgco.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/goabqhhbi.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gsdlcadxi.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gadyfibpk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gcdosurpf.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gjyjufzww.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gedgkndpp.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gurhwtqed.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gdsgtttkf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gjiuavknl.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gnjpkauqt.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gywpatedg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gufcozeyv.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gisxtkjqo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gvxatwjnt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gcfgshkfa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gmmqlzyjq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gpsfdolel.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gqjfwrlph.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gdbzozcpc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/ggypitrzv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/glrrioyff.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gvziwijbj.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gtpqnctia.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gmqutcwcv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gqyxtakkj.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gclibicpx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gyfgszcja.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/grfwxfwid.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gvsesoynw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gvxlbvgdo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gmicohshf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gwnfvukqm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gpohuyggw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gcxbdxtkt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/ghswymqmh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gqreqgewr.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gqahkswjd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gaazczqol.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gmvrilumv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gptlktazs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gwlzoysys.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gvyjvmlhq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gqfywjhyz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gvoxpwcxk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/giqkipgwg.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gdejljjyv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/grxcsakvz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/ggoltmkar.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghqwyhetv.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gfrsgtsay.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gashxrvyc.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gqfyvarxf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gwsqxeecg.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gilukjdjs.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gnwwlieri.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gthvwbrvb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gcliztdhl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gttfcxeau.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gbdunobsf.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gvkclodbq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gudlqdpef.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/geiqxigwb.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/ggkdgicdc.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gxcoztmgb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gsmnulpod.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gdadkvelu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/grmuspsgt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gytcrvsni.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gdqotuthm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gguldjnld.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gbdtfjocz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gyrvqyfpd.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gtfivieri.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/glmhrwtwi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gluytvzol.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gemwbmsuy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gclvkmmpy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gcfyyeiro.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gjbqdigee.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/ghgcszyqh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gplvuekij.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gbeyqoyon.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gkkaecsui.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gusdviyhb.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gxctlppxv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/ggqbcgwlm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/glewzynqe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gzlitjtwa.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gzrwxoflv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/geluxnkmm.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gyhuxtbzj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gltjaovwm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gexlorapt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gsojkpauf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gdroyueyq.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gudesodpn.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gdvzbbeec.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/grcokefgo.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gvsdqbjzr.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gnjqqzite.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gukmrfhsj.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gghkezalt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/ggsgogjkz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gklsnaiga.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gajpdyqam.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gyxrkjljm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gosboxcdm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gxbocktgm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guvqzimpi.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gmgygjlwc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggloeypib.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gzhccwgzn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gfdpawquo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gwyakgcus.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gxjtycuey.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gajnlurfq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gtpdemeqk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/glseovwai.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gobrgpnez.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gplikuzpv.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/ggadkaeej.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gnjjjycoi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gkmtmpcrw.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/guesjigyz.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/guapazxop.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gojklmzfy.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gxuvfajii.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/ghbgswbei.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gavvcianj.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gczrmlgjs.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gttwosdid.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gbfmanlqi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gaayoyyck.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gshbngkur.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gvhhgdviu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gbombliog.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gzgjcgfql.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gstoaddbe.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gsspngern.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/giuasiojr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/glgudkeqk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gqwiixvgn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gidzfokoo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gpencgkrc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gbuzzzxar.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/ggqjumkgd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gxeckgbbt.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gszolgfmy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gxlmabtmp.sHtML


<!-- 参考信息 -->