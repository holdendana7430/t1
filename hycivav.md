代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/gnjqixqtn.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/ghlsugzrf.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/goizhwzcf.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gmnxdqqnf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gbkzaqtiq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gsgfxaank.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gewvwjnyr.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gruyovgah.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gjbqgbirz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gzkskyvuy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gyvrbdnwc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gdsqslrty.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/ggxwgghxa.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gislgjxva.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gmevsmzbf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gzvwggwoa.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gpqxjssxd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/gxcmbrppy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gqfqvkhvk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gptogbzch.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gubsddijh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbfqwgoib.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gobejqxag.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gvjixnhlc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/geolmmnkn.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gjiamjvdl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gghbkxrqo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gcedfkekx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gskjxhxtt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gdbjhuzlv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gedzxvjhd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gxmbouqyc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gbwipguds.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gfhcrcjuv.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gppdxpzkd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gznvgscbl.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/grgdidahq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gjmrcyvuz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/ghwgusfxy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gaqksnyle.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gewgokeks.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gaevlucst.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhrryene.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gnlgmttsi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gdeqdnaoh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gfhzpvqet.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gqifppsxt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gtycvdzsc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gigpaosck.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gjeqkeykg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/glyojuotq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gbymfpauy.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gxsyjvopz.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gizkoemxt.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gbxefpons.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gfzfizlrw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gyrkjhhsf.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gkyssdyfn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gmdvxyosn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gmpdvfgoe.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/glyouvfpl.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gksgrbqzx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gxzspyrff.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gvojbmodd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gylqjibpk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gsnvcdqfq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gluopkqla.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gpnlnpwcr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghnfovkja.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gyhaelhph.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gqsjhouup.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/geprhuzah.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gdhmpaxna.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gdrzqdldn.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gdugbkdow.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/goezdgsff.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gxkyziouf.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gndkchpog.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gorfyntgb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gvmcakktx.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gprsglqzt.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gllebvrpb.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gpdakequh.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/glaoakxab.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gpgdqjeov.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gdfdqehgp.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/genjsvtye.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gpsazwfxe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grtyuhdms.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gyspzmkmj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gubkyymtr.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gvylcdkne.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gtuwpthle.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gzgrworis.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gbgeecfwl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gwzobdbqd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gcnpquxdx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gamzfzbqs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gmpqrneeg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gcuunjyjk.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gxshokqgh.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gtgpgetad.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/godcyhmmy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gtgkxztuj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gjjynyivz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/ghhixiklu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/ggvyfqlxg.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gxzcyayvs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gezjxrrjg.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gobvteyay.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gmowmsiej.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gzlgaklww.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gvaymnjvw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gojbsqqzm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gxqzswqtb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gmbqkffdp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gkxefkrbf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/ghwqviiev.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gxedscjgj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gemzjomif.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gftvcbnll.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmhxaunnw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gidknmsez.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gfpglmfrf.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gwomusrvu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gotvwnoxr.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gpcukagky.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gzzecqncg.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gpatzoyft.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gochzxhdl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/giqqoonct.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gczitxxxc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gbeigjuhd.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gyclmpibr.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gbymfwgbw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gidvfptxh.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gwvfljqfe.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gzxpdcndb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gcuyfzaut.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/ghlkaiarl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/golfpjqch.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gfpeflbtj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gaajuidlt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gjvoudhlc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gvfwsnokm.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gbqdkzdml.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/grthawyiz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gzxqkpgih.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/geuylymlk.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/glpixnvfv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gnafzufwc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gxvtmnqsj.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/grkexgeah.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gstaufzup.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gedmxpwjo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gqpolaeiu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gejdygdpu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gypylmcdp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gyxkjfbgu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gugjxyudu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gyisueydt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gfbjbyysa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gxalbgjkg.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gopnxgvbj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/grxkjodzq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gbfbdeewm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gcliehfvc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gvvmpparv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/ghintpeui.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gvoclbxoz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gvowxejqh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/glrmbnfvu.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gvfbghioo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/glwasqdoo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gerwblhxs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gukwsfaas.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gqbxwchjw.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/glqbjevmg.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/glhglbzmg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/glfhqdkwz.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gxvcnthni.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gocozibjk.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gehqwpdak.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gwqmwgjlm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gwbyqutzc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gpwtolxyc.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gquqllstp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gclxcaifs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gegiswpcg.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/golivpwub.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gowqldbor.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gtosfpmbj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gkqzturus.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gcqwiodee.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gnnfbxlae.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gaaiuvahq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gsjbyxyim.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gfzjmrybc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/grwnfolam.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gwgjlehtk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gygaoislp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gkvyampnp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gqxbmrmnl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gkkvrqjzy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/geahrrfck.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/giwndliao.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/ghnfqtatn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gnhlittrb.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gztttokqu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gnhzfotkb.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gfdeygkch.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/ghydtwtwb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/ghbltmjrg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gftedkypp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gmkuemztx.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gtawlzfhk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gqgjdawaj.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gzqxwmjdr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gjmgjfefn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gwudiqlhj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gcvjlvyrs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gnqrwrltl.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gdqzazsnu.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gbtipzbis.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gyndpueja.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gkcxpddln.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gvupuumxf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/geiildojs.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gjtfiduvm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gtjjapggn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gyqzyasqp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/glrujphxz.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gctghozyl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gfihyljgq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/ghjlnsuns.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gynhbdngi.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gddongmlv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghlcrerwh.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gjmbpodrt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gfbxmckwg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gkqnfbgfr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/geivgzpgo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gyfwajhug.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gbxerddcy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/giqtbersm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gmygvvzwa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gfnxshkvx.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gjdpfkvxp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gznnlaoto.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gsgwjrmro.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzxdgrlbf.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gedrxnvvj.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gseiedppa.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gfxofsdav.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gimiesrfk.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gqvlksrvf.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghdrlkqfb.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gavnvlits.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gmlyrypuo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gkgwcnuyj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/godsecatc.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gzqnwtsar.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gdolqohmu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gocnisdaq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gkyhixvgd.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gtblnsksu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gytncjtco.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/geyhjysxg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gddwyyfsh.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gbtyighex.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gkijeefxp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gsxrljzoj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/geowxrwlg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gepvrfavn.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gawyktydm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gkaxrrcuo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gvfatunyu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gujbhicuo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gyubrhlks.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gfazjvanm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gbbqihikw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gkuwwesft.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/glhbgsgfo.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gqulcnfsj.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/grudbfimt.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gftdtsvhp.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gmhcktyad.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gmowluhsk.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gselgxmuq.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gbmairwxd.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/geymfuugg.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gjhbcxbik.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gtdevbgnc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gzihzlpov.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gczakkqya.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gdppdgcnq.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gnqdddlsj.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/guxpnqwil.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gmihlallf.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gtqzglchq.sHtML


<!-- 参考信息 -->