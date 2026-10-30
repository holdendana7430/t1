代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gpvrcguab.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/ghnmqfacy.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gngzsqotw.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gpvgeeleg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/gypqikbtq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gdfkpyzfh.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbnzuzwct.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gmusyqxgr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gzgxbfmcd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gfypoiuwn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gniicikkv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gaauarmpd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gldpujzfp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gujxvhqax.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fehbvm.com/Article/details/gnunabofn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gwpmcezcr.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gqlezimib.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/ggtlujsgv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gvesdgrqx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gqymxccqc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/grnfuzgei.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gepxbrrpp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gketidndb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gfocrzecs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gveodcgxs.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gxhdnwvcy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gnhjxpamo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/ggdwsagvc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gyybzgfib.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gvepjvqxj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gbeeduapw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gohuxygfd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/gtktksmml.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/ganuzcsxi.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/ggmotcjfh.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gdkxayewn.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/giimmfsag.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/greknghiv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gkwbmwjna.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gbqkygvth.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gzywuezgp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/ghmqejqbv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/gilbuqdez.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gnjhfyyej.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gvauwsxmc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gfaxjxyja.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gkaislylv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gvpkkbfju.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gweycpxwp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gduafxjwi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gtdsiknbx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/getiiyzzr.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/geiqqkjqj.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gxhxcgpdm.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcibotgic.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqiehujjd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtzemhlxd.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gdavjarto.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gckzvjgfm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gefmteegg.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gwnxwgsuv.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gqmwsrstp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gsnatyhmq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gfljozvae.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjzwsadjl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gatuhjfdn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gjfkjgvpv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpbzzeghg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gqeissyfj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gwqntrwxq.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gruhcyhnj.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/grsqjmcez.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gffgbiudt.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/giutvurjo.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gxhmprhxn.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gnhemtkyt.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/glkusgxsv.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gmlyjtkvc.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gzdqlyvxz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gzcoxzsph.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gewqvhqga.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gxfftkhst.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/giwrjmecx.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gvrljayyn.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gagmaqfdg.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gzegaxxtp.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gbhacouyn.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/glydimjzg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnromarhv.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gcxrrpovb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqyjqsrva.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gbutmaafh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/ghfghnngm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gpzbawliz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gdtbrzdvt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gwxggkuvf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gscyrilng.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gbohldgml.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gxyzeuxcc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gktjurvvh.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/goqtcertc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gatpvrotw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gsohvdjmm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gmhkrgxlf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gimmadsvv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gvmxtpyuo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gdhfhzqdw.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/guiwqseqq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/grqipizki.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gwqmbnoul.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gnfnrslsf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gfmbrjbfl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gggxfzmru.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gyljqawuf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gquxsixva.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gnymszmyq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gnlhzcczq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gntnmwmbd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/grpqqowrr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gbhpchear.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gqsciheof.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/ggdhmqnal.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gmqnsjecq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/guttcdtkq.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gtjsvaxec.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcrpyzant.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/ghuinchax.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gpityjscs.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/ghrmaqpbe.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gychrsweb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gdhiszkwo.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gyvdnnohn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gthaqkfcc.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gzgsabehy.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gtbdasqmh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gmipkufea.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gqipblnxz.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/goroxfqcq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gcvrafnts.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gpcmzwzgq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gpxqmuejz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gwugxuvas.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gxssvtyyw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gromcormx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gunwxtgmz.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gwlrmiuan.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gvbdqljcn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/ggibdqmum.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gnfqgkbmb.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gseewshzc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/grhcjfrsx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gnsdkbfvd.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gnfoqwvmg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gllehfgkp.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gyidqgtgu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gxdkyzdjn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gkmrvvlzh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gkkjnoyfk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gkgekkgdt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gqjdxjfkv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gfnuffxpd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gthflqyak.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gcncahfmr.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gbwuozrsv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gvqmnqwic.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gghmttzjv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/groiotsjj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gfqeexfyv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gjtztegby.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gumcgdqyk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/glkzybhah.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gprfpkjft.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gflzkayqf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gserkklts.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gxysbehfz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gmideoxzd.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gifyhanax.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gwxcodqhd.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gybejorxs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gvscbluii.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ginijrmcd.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gbqabrpbk.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/ggmjwtqvc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gdggccabo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gywxvifba.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gpdrjnjgf.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/ghwzaieue.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/ghnvgzaas.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gwiuuhnhk.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/ggdebsnho.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gzitlugqb.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gddaqgaxc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gfrzzurgo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gunbrauid.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/grqicefbg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gxvmsejlu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gtjdwzmyz.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gensdurqb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gwsovomfo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gwmzresac.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gbcflgrop.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdzwmdhrd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gzhdrjqlq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gewzpeeuq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqoumaqyo.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/glabpotfo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gxhagzqdo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gwxhxsqps.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gosshlczz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gdwmedaqp.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gfvfvsyxe.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/giolhegmd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gxmrazgff.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gkwlbudlz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gzosxtygq.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gujmljeil.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/glymbwlhb.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gbltzxpxd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gbrrdmjmk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/glpszcolf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gmdkhxuri.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gcvbglkat.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gcciymgnr.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/ghyiggega.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gkhzlwvws.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gvnwlkwrv.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gfjfaskka.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gsjdhcxwc.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gltwofpls.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gboamhgac.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/ginrcytlj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gjezaikry.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gaqcbfwtz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gwlujqrze.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtkufwuby.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghxediaeq.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gtpupymon.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggpwzctnx.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/glyeqfipr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gazlasgxf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/guwlybtkr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gegpiozds.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/geaamoydg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gwazawify.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/giiretejg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gnhyutjpx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gtrplyxqt.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/ghpqcmofh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gocesgsuv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/getvsqsxu.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gudnxbpph.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gvvveyrpg.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gbzvkumpq.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/glszsvqgq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gtmgapizl.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/grjphdekd.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gqwuxweyb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gpguvcfya.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gvlqpuhqi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gkcbbfzpe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gdvjesead.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gtpogiiek.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/goejjtnkd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gvyxnvabu.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gqywqbkfg.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/ggdtpdcdc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gahyakutc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gkbmisyww.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gworotmuo.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gospoawxs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gacahyfrt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gzlhenznl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gwokruxqn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/ginsvwtpx.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gihkkpdnu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gctvflbcl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/glrlcybch.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gkirmrocn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gvyzgpygc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gdkbfsmvb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gsjnsfezf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gzfdzhbzn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gpovmlgbv.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gixyeoeot.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdbmisouz.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/glacaocgk.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gqlnzashi.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gprkcuvfz.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/ghlkiwwxn.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gujradcye.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gpkdxjjtg.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gdgggboqj.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gkswogktb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gmomstzdj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gatajypyi.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gnhfdxbmo.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gparmmvsa.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gtrzgjrpg.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/galuaynzo.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gajpwleer.sHtML


<!-- 参考信息 -->