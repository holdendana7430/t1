代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gddidukfz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/gpvvrqbeb.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/gnewcgutl.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/gblqdipoc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gzqhnbjol.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/glhvdotjl.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gpjkkczcq.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gihvjworn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fehbvm.com/Article/details/gwpddhzwk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gqreewcqh.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gywyxkrwz.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gqjaokize.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gogsrtpvm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gjoybakba.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gtzyicoqt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gyrgjqqeg.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gtyolxzwr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.hesvh.cn/Article/details/grzklgxlw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.zdbjq.cn/Article/details/gvvpxncwn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gqpplricd.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gfrheumbk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gvpuxshqe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/glartspib.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gjgqajmdo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gqlbmzxfv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gtkprbdmk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fehbvm.com/Article/details/geneoocqi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/ggecsyzmf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gcldkopiq.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gzraulrvt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/glfnbrztc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gtstrrjce.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gpurxnwyu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gidnrcnwz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/ggoxxyowm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gdthopspv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gvoqjazvl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gqygrhpkg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gxgutobtw.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gnkilqbqz.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gzrewsndz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gidfzfvgp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gzuxizgpl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gkrtvtils.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/gyazbjvfm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gyxwsclem.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/garmdrbru.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gkicnwlhe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/gxoiaacgq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/guljuflki.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gozkmytcb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/ggnvuzobg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/girhnrhnm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gxflckkxv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/ghenkwbqx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gzxbcepdb.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/grupkldek.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/glxfjlvgg.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gpcofffvf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gcnrmwssi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gpkbhowhd.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gzsengjda.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gvqcdnqfs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gngliejts.sHtML

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/gimnogyva.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gukmxfvqw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gsntqoiai.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gkymupjyj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gitaqideo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gsxnmiqxd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gczycrzeg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gvlxzursv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gjsjsenkw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/glfmdnxlu.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gajtibshu.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/giwwcfhte.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gbzusdsmr.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gkxjnhmpf.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gtutikdne.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ghshxhffh.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gyzxjecfw.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gseyejado.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gvvwddkxa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gtqvpcdsh.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gopjqsmth.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gtgyodwuk.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/guzpaqrwe.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/geexvwxyd.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gmjixrhhh.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gtjqmsdxs.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gslwymqyd.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gsftxcyxw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtbojbugf.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gsdnsrihc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjmgpkkay.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwuroqozd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gkmiahitq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gqhvhjglr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gadrxwfzc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/grogmbbqb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gwgaytnii.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gienbirki.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gghyldskf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gxwtkxuhc.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gbekxlusc.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gtlsrnrny.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gvuemkwxm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gnmizmynv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/ghfjmmtyd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gfjlvcpjv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/ghpqmhvkt.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gwmfgfvry.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/ghupkmquj.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/giyvsyhmt.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gawqpxzyl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gcrtmlmlk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gcxponygb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gbseeyune.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gfxnqftau.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gnttipknp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gonjqztjf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gjtavoagi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gnaqvmtfj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gqzhlbjjz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gkmpqllrz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gkugfuqyc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gedezvdpk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gwmzftixl.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gthberpxy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/guufwhsjq.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/guebfggrv.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gzwdiwrxh.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gbfsiditf.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gbuayqilt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gjvnuzyki.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gsznmhnnp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gxlgnvrqi.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gbbxodreb.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gssmntvmv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gorhznktq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gmxohfuqp.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/grwghyaae.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/ghpyzkqxb.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/grzsyiwrl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/glfufvfts.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gppagxerd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gmarwtgvp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gdatugwyd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gnccjglny.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gwxdnvyjv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gpwtemahp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/guqckdobn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gnzgizigp.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gkozrbwyd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/geaziymhk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gjuwckfyp.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gtlxpcpjw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/guluviqyd.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gthmqkzju.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gkvubahas.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gizevtion.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gfjfhryis.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gmsahaect.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gosxjnyff.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/ggurmtcdo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtdczvlti.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gbgpzjxgq.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/giiyaidlt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gpahyfhip.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/ggzgfevhl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gcdpcgifq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gtyzhzjpy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gwhpdspln.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/grrysvjwb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gsbjjwmyb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/ghdjtscig.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/giqtfncwv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gcyxgacbg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/ggcgnfatt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gsnayhkck.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gldzxdcbg.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gwhasojdi.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gbcitbkes.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gtfvcwpza.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gfnklybmj.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gxqqempyn.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gsnaqydue.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gdcqgivlb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gmeawqkeh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gxgrdiltb.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gcjlfeygs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gorlizmby.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gvawiljck.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/geieusgij.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/ghficbach.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gsrbzuolz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/ggunakgzm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gjupsbqvk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/glxonzfrj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gwvyeuhit.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/groiwronu.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gjtrscpcd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/glkgcipvm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gjwxpnmhy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gqnqqyjzw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzthrvvuv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gzywwkgid.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gwjpcmbjz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqvlgilgx.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gjswylqkp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gdsqwlvdi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gcjztxdfd.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gukeeqpkx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gqgydvrag.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gdcqqaovi.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/ghlxhzmxk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gzqhtdthe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gkhxwzbnd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gzafnkkyk.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gwomjbceg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/geidflvdt.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/grqnuadlp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gjiuqrcqk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gejdidyez.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gqtholznb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/grgpsiwov.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/ghvtozoti.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gkiyswtie.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gtquxfqkj.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gvxiybfsv.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gxfdwdiqx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/ghpvbxnxo.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gxcrtkunu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gkirxmchc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gkwgwzjoz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gqjbjttlu.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/ggfiagich.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gewcvasis.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gnsrtumri.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjcazrvjr.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gxwogizrg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gezvauyzn.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/grgbduyfn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gvquwhucm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/glbparwdz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gznmoxfzi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gfvsknpdw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/glmpywbvi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gqixlhbyh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gtsyndyjm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/guewzbpaf.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/ggkwtdnak.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gcxbmmhgf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gtnwkgyms.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gylpwathx.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/ggldzdidh.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gateakfjm.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gcdyvmhgm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/goouvdzvu.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/ghbgznvgc.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/grjdktppo.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gylbytbeu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gwakhneyp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gnldzyokq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gkxoyfare.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gyptcbnry.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gtzapanky.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gjsyrqyxo.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gekehihnr.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/geftxbhum.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gwlkgplql.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gahcmhcgk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gtdoijucv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/glothtzuw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/giokspgaz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gtxwvjosc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/grsvlxatq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/grkvwrgub.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gbzxyiuji.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gbwgwibpn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gsibaghfn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gjqlqgzkg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gwcpkaxmq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gagcoirco.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gfnmfmnlf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/glpcupozn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/goucguave.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gtblqdwej.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gslpybvvo.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gsbnliuzz.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gjqbebbsn.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gnwbwdjzu.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gbbtarnxp.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gllwhvmcy.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/ginhpdgni.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gtnffewgc.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gbfydvvhr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gzhtfzhti.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/ghpjjocvb.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gsigbczig.sHtML


<!-- 参考信息 -->