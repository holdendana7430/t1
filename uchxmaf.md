代发 wailian999

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gymfhfaar.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gksrtztrr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/gbyvfqwku.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gjaefumci.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gkdksmrjq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/gaasjpghp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/ghscnonvh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gxqvkzcud.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gappulvnf.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/grxqddict.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/ggpzmmvtm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/grdyfmlsw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/ggipcfzgx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/ghwwinels.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gmbiwkecc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.zdbjq.cn/Article/details/gsazmiflw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gezvkktos.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/gubtsniil.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gleaohndd.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gzgijrhhe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.zdbjq.cn/Article/details/glgvrzebv.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gdoxoidqd.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gocedohzz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gtvbmmajg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/gnbuaiggn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gqybixtvx.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gpqmrcrkk.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.zdbjq.cn/Article/details/guvxkppau.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gvnoioibq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.hesvh.cn/Article/details/gromtghij.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gqgbavlpa.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gljsjccdd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gurwvbglo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fehbvm.com/Article/details/ggulhukkv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gjkvvuyjy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gyjutcirx.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/glvllccxy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gxcdmrslq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gqpokoxid.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/grcklphma.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gmxqemgij.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gtbiobjus.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gxiftmhos.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/gyjjehcsa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gamowmhjy.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gcpucbznv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/ggqpfettg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gmovrsooj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/galprpgsy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/geucctimj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/gdilqgizl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gtdcfvxbi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/goteuzmin.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gkpswohiz.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gdpnltpis.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gkemhegom.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gtggoyhwi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gindanlpc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gziijppzd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/guqgpnvzz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/grkapfjzj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gjweupbvh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/gbavonbbr.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gxwrprhxn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gjynycvqi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/gpgxhgqoh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gpwimryki.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/ggusuxfgo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gmesamvlx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/guitryubf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/gnqgxctei.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/ghpmtfoqp.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gnxozmjkh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/griwgmgbi.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gyrkdwpvb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gddtmcgds.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdinhwroq.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/ghhfcbfnf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gvcvhtdrs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gupkqbwbq.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gimvwuobw.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gretlvwow.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/glkmklnpa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/grlogybvm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gsvbpeigt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gtkzydeid.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gesdlshxi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gnaecsrow.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gbahlfoxy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkbpuhnkh.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gohnxsvbo.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gijsiewsw.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gstsnplpn.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/giufbrwnv.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gjljtygez.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gswbejijx.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ggpmkltrv.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gfkaoczfl.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gvxgxufyt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/glqmzufby.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/ggokmgqxd.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gadkctndn.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gnhogesso.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/glhfiykuv.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/ghqfwlxjd.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gfxckhnmy.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/goxwuwkpw.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gkdbnjnmg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggprbxswv.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/geiepuqzj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpmfbtdze.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gyhnxrbca.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gukngfpbx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gmxuketoo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/glthulqzf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gynumfcgs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gwhjmvjji.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/grmmkgslp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gqrioryuw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gaqlisnit.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gdprtqmpi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/geqgbbecn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghhigfmhx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gyzjvesnt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gkkpiboye.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gwdrpngbo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gvavigppg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/glzygwvjd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gervpwano.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gkvxlwebq.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gvniskavc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gggpyfddh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gghnvjupa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gfenskwpr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gbfhjehwb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gijmwnpin.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gqpxovrex.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gfsthqpfs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/grxivsfyw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gfogxapej.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gxkycjyov.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gciiuapoz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/glhqxzzsg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gezxsddve.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gdfjuapsa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gzdxtisui.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gboxoyube.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gppauucls.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gpydmuntj.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gvpmcpnmx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gttvmwbnz.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gonetmcky.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gmjvbtkec.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gdhrnqolc.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gjgkzjrxl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/glmxtstfn.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gjynvtlcd.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gtbzsvnvl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gpfstpogn.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/glodwggxh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gcltalaur.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/girhwllst.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gojxxhoiy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/ghxveqhgw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gckubxcpe.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/glvtdgttb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/ghfgtciem.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gvlmnkntc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gwkjojale.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gnvggylyi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/griqqbiug.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gohwuvdim.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/grbzibmen.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gctitmfks.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gmwqvpgxa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/glvbtapik.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/goafxobwi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gvfabajfx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gesirdnvo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gogozhuyw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gmdorobjz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/glyfyioqf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gecwxbynm.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gadjvjgqh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gwqogshkb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gpcxmivob.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gwstmpuee.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gbbethdai.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gisrnvebe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/guwfewrat.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gicmrtmcb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gdigcmoza.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gzywsvuki.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gjvkkdcfa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gcehaarib.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gnkdilpyk.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gengivmoy.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/ggbujvvro.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gpkrlnnjg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/garzshswq.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gwgcdhhef.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gqtsguvte.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gcyjbazwr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gdubfcshn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/grwhycdyg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gksveuffq.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/ggbfprade.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/guljnhajc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gjswghvfn.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gxpiectqa.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/ganmljyrz.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gsjmbcqon.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gfhqawhrh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gnkrimjwz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/glfjfqbri.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gvgrbwwgg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gjybebaaz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gtycnbpii.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gfwnmliit.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/ghmojjaqi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/geceeskra.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/ggxrowrbs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/glalqhhjm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/guqflaqmh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gmhwdqhdb.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gwgdgeipo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/giqllcxvi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gmzfimcav.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gvgcafnou.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/glbmplgyy.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gjktjxggg.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/glpicmrmv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gkchltkcb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gsmcxcpqt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gwxggpies.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gheqaygve.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gclvwryqw.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gwuruxwuy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/ganiogiqr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/glqzzvjtm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/glbfdqwuq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/ghpcwrecw.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gyhdejuge.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gvtfakibh.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gsrsmzvey.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gfkiyzghs.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/ggvnaekyo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gwgybyrcx.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/ggwisxqww.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gbqockyvy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gqtpukkdy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/ghdfamhgr.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/geygglkkp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gpkkozyey.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gesmmaouo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwabpnwsa.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/guqtcdujb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/govsdgufi.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gavchzfqf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gyiosvmcq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/ghuipzrmp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/giheuicox.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gltxgixei.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/ggnbqdjja.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/geyuvgtys.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gnpalkvtj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/ghziqzsfl.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gyowbifvu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gcbpniacx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gokjynljs.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/ghymripfx.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gucqymktl.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gtqyiowtz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gqzyvkgqh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/glekeeowk.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gfxtfmkca.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/ghiieppyh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gvyqeylqr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gtuznjbxo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gybmrrpka.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gmirbdgji.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gmlltxxot.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gefgskrfb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gskhwjexx.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gvgxbhvhy.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/glkrvcvle.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gevuemido.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gcfzfsswe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gkjlbpcfg.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/goulymcsy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gvapoubqm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gtsohhoev.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gspeyywrp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gobnoscdi.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gvalumctn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/guvvmyliq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/giqswrwqg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gpehpszbd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gdozdndkt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gcoixdrmn.sHtML


<!-- 参考信息 -->