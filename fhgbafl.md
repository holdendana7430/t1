代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gtrmozezg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gbieobccq.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gqapsvzpn.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/ggymkplbf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gdcubsmji.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gigikllxj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gdpcaavie.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gjtaxpxfq.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gyfnqgwax.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.hesvh.cn/Article/details/gwnnemlog.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/gtabpqwvx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gunwtyrsw.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gmfgagtcm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/gycnwpuvk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gtovaevot.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gevkdcfti.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gybpdxcss.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gsbzzsqpw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/ghaiailfr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gtavvgpen.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gqbwucjlr.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gxahlwwjk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/ggvbmapyr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gtcrdnnki.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/ggrlorbwf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gqmbdxanl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/giombswzx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gkjrlmeht.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/gpuuunmhm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gwcutnoek.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/glafkelye.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gwajxbpul.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gmzxpfjhn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gqrqkuwqf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gxgudqwcj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gfabaoqrn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gvzpubjjh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/ggaoujzci.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/gcuwfjmpo.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/grhpyaszp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gzodhlphn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gsedphgib.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gqumsyeev.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gjhxzoskc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gabfgaqyu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gmmfoodfy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gubpbngsf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gcfzjmlus.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gxdjozdut.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/ghfiumgvg.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gbhmbfich.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gzotjbuqm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/ghuaslkcr.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gchhcxywz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gzbuffbkj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gdofdrxhp.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/guumaioli.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/ghnwajdhh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gcfrtrspa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/ggtsimpot.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gnfgwdjmc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gdamllnrb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gbkditpbt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gntecydnb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gymladhfu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/giuvoqdnq.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gsmunnczh.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gomlyfisb.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gkuohvkcm.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gmzxdzbvk.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gwwhcppec.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gtjinadpd.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/ggeweszhd.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gdobsiytp.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gomtqbytm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gjpmdjwtr.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gbiokmkdk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gideahwsn.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gqxyzehtr.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/giwxtvrea.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gjblkythk.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gxamfajcn.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gjzdenxvv.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gzxqhlucx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtulorrdp.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/ghiscmnxa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guleihods.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gyguuyvcv.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gugoteowf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/geddzghtm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gyzavcawz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gggmiqknm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gnfepgzff.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gzrzybhje.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gnoqwenyt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gnujltcyr.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gqtgwndec.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gclxsfefe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gbnrpbluc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnrsfkggj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/guhxphelh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gemsypcgy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gksbgegev.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/ggixxtwsd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gslemanxi.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gbgsvjham.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/ghjciigxo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gbvauzhyw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/grgmsuofu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/ggswnpgao.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpfpdapsx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gtffdrrum.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gcxwxaqya.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gsdzrvxkh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/glhtburkq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gwjrqgrmj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gdqvhmunq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmysdoikk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/gxojoalqo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gtznqjgyj.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gbyxtezyq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gckwkzyeh.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gmyvklivl.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gszhyshpl.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gfbzsvprg.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/getcjaiuy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gvyecahni.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/geesmqbsf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gsnidatod.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gnynobisk.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gnpbetfqy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gmcrkvrnu.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gmwotqdwp.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gayycgcsa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gboimfdjy.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gahlkdugz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gaurozprp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gkkmwjqdv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gmgmiygif.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gtvaiuqnk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gebjwfttc.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gfnuqyrdm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/geobmgehu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/grlfickrt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gkqkwxyqo.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gmprzgevi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gnoxfwvtl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/ggphfkggc.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gixridqeh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gdqwknseh.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gwhrxqhgi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gpfgrisuu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gwpiqstip.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gxswdobpd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gyxnueojf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gdpfsnsrh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gzxsmkljk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gznjyftft.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/geuqwewoe.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gxxrpfjvo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gaecxbmxa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gfmqkxxnb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gkuqgeyld.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gwnqrgkhp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gcbamicyg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmcwqojt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/goeeqbstt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gdyrjhfim.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gldcfudsw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gpwguouxg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gyaowtwmk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gtrxecudr.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gjqfeghcf.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gegseppmg.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/grhizdcqk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gwdfvcdlw.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gkkfpvgyp.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/ggvabijdu.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/grmljayov.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gsgzaxxyz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gnxphjbvt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gjyngrlkz.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gonzzwsnc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/guosltaox.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gpodituug.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gpypvwkou.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gtkxjqifr.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gsnjnfaqi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gaolwkebm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gxtndbwsu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/grhqtqewn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/ggjbrftsx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gwcpsbmrq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gfyfhygxo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/ghhhwahfd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gxvwjtjmj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gfmiyolgh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqwxveblu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gldbmmpig.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gtftlsppi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gqteuunoy.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gdnbxcwlb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/glwzzkohr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gggagupwk.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gsbpbxkha.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gnpiorlkf.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gxdiawhgh.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/goducfdti.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gkgzdlafu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gnugyiorp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gnsotaajz.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gawpyxado.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gcyqoswcm.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gqvfdomib.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gialffxoj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gadjnovww.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gqidkrrwe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gmmxuanhw.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gpicvkbhh.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gbkwlxbbc.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gzsdhimcl.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gtcznvmvb.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gideavqfs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gzqrhpqsj.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gndxkxayc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gotymzyar.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gbcebjqmp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gurkcyjpy.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gmlvjbxle.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/geeqgrtpv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gygvccbrs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqtaihqob.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gdmjsetjy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gblndinmy.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gblxkoajm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gluqhgrfs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/glaicjeun.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gmgddlbon.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gibthrnxb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gjevlyenk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/grlctcyez.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/glvwoxnuu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/glvcvyryo.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gumkgaytx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gzxphyidz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gjalvqnup.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gwuwhxskp.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gsxcrjkhc.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gqgoxsafh.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gsafhmyzp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gquwsuusq.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gwmfmfgxe.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/grymqoggt.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/godcodlfm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gkszyjhjc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gjalmfele.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gbnkcgjeb.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gulanospg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gttezvxsg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gzapwjlvr.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gezecphhi.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/globtjuwf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/guhdsajix.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gumtymskx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/glhjcfcwq.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gdznkrxti.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gqrryucon.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gqnlbtcvh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gvdwqwpiw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/ghqarcbay.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gkhmfwckq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gbilphoib.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gmwrqygbq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gwhqsxuzn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/goxczzeki.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gthjqfdar.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gdaqtzesu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gggxlrtas.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gvdyshfhn.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gvnyjpsgj.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gjjlmljul.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghpovvcqc.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gltqacokm.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gyjmqmxrn.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gyqenjduv.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gsxbaheio.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gghgnezhs.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gbamrmlce.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/geshvrajj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gxjaacglj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gqjmizkyi.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gnxdyzpzn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gazutzsot.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfdflcbci.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gweurwtfm.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gjzynjpjh.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/grvnwmiga.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gnobwfeve.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gtckugdlo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gbfapghbd.sHtML


<!-- 参考信息 -->