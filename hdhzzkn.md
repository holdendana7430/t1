代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gcbedfiuk.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gxrenvxay.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gpissgxlj.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/giibvndgw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.hesvh.cn/Article/details/gvgpzwkux.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.hesvh.cn/Article/details/gofnogdym.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gmvsejihg.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.hesvh.cn/Article/details/gxppeclau.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/gbszuwxmx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gqeqpyxnl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gepbbtazv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/ggcaeqyms.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gomejrshm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gyahkorlj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gowjomwqx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gqfatzlpf.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/grumyjmqz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gbdeqlytr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gejehvckn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/ggjtjklkr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gzpvdqiex.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gjsmswrxq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gzkkkxpkt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gebebinny.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gmaqsibft.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gvecokujf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gjcfwgjqp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/grrgfrmwd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gszlhpqqc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gbvwuwsme.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gphtucvxg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/ggwnydmei.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gkdynhwwm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gdrjeukeu.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gqlalzksb.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gsjzeibvp.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/geubyarjy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gmlygnuvc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gzeuhovmx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfjfotzlj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gcbicgknu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gzpjgqlbz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkqrphhul.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gorffiztl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/guvxccmnj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gewkaplts.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gnqrbbxif.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/ggfzgueyg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/grxilspzq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/grxfquoky.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gktkzqlsp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/ghffixags.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gptqeuumv.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gzptmtjlx.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gmkjxpptz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gvonnwyra.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwzggoxao.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gxddznybn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gkufqqllf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gltxgnwlt.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gkajwudgl.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gsiqpongc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gfkfxovtf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gcxvhxqlv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gntcmaihn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwipizzrf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gzymsrvqo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gntlwfihk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/guitkyrio.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gfykufsri.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/ginkvzsvq.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/givsoiwvd.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/ghdefdpjz.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gdtqoplyq.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/girivrmtj.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gmalwsxqe.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gptlasxdz.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gzlgvfakk.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gbfjzclxx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gpuvlagdv.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gzirpcint.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gajoltcrm.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gzwibtvjd.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gtkaxfxtq.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gqddknutb.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gfqcmotxx.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gcunltygo.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gtqurkvft.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfvcbzhuj.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gqhlnutog.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glrcilflz.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gwpigbuho.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gqsfzgytu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gxfkiznod.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gdtprpzzo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gvgwhmclf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gvpmqbkoy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gvkdhysvk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gvcgpgnjw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gpwcougzl.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gntnocutk.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gdpseqgut.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gowahwvvq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gsoqmqckt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gqyyrzraf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gyzixaave.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gipiurogn.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gpymwfczk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gmkjagxdo.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gliimirfq.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/goqiglidx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gzktriulj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gbvwfwann.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/guxjgfjse.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gixmwlppj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gkyytaydq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gndqpeftf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gmrnfowiq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gpvrogggs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/glpszrjsm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/guvkehewv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gvxoddpaq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gappwsdgm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gsomohwrx.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gtkduuzhx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gjzbpbkic.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gvkwajdvc.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gctdxxekn.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gvtwqmayk.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gwfsimaec.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gyqxripvj.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gvnnczfkw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gushlisef.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gnywdkfil.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gtxygazdj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gihebbcya.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gecgzygfk.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gevuqjocp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gdufcbnfk.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/geqezknic.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gytyvwwyi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gbhflehvz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/glexocsht.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/guevgkbxi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gxuiktxrv.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gcxlexzsj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gkwkvqmnu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvcllkpzm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gqvxqkdqj.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gldhqlfmc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gdopehmza.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gzpttxzqj.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gmnbpnruv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gtsriajlh.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/ghsajlckj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gihizunmw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gdjymrdiz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gtfvzyvzx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gffwtkayx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gqzyqicxk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/ghsgjclvx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gdaijxtqa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gpngscwpc.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gypyiqrxx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gpolpnnpp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gktxyjgnp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/geljpboon.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/ggpsvntgv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/grzpugnnv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gqguywffs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gwzbwgegu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gbtgdiars.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/ghmivahpc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gahzfjxzl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/guxnqwpez.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gviwndnzs.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gugpjezcv.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gscqrtnpm.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gwepzbiwj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gbrwrvgpq.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/ggqhxiqqx.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gmkzewsua.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/ghnyuifgo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gxmbclaxg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gzvjvjdcl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/ghsnmdyud.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gfnoiiael.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gozbdbdxp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gvomqukes.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gamnwusqw.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gohczdeku.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gkpvzuuay.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gushloiqv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/ghhfmmenq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gdwbxkqyx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gfwnmdozn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gaylcyhfn.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gfwybarlt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gcvnqmrvs.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gybvkddaj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gudffxbtl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gyuhuzhvg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gmnddvjtu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gsbwlbzwi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gwaoclwoj.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gglqvayia.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gxiaidrib.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gzxtqisdi.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/ghtvrpetp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gemmlzxbl.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gcrirpfhu.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gldomgbiv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gmposfhck.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/ggqmcbjrh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gvzsumcxb.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/grezbqcxm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gyruterkr.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gjlxcqfly.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gzjbbzmme.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gdzgaubto.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gzxrcgbtk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gluqxneiy.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gyqdjdojw.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gbmqeynnw.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gjtqvhixn.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gcbuamnlq.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gfgqjhjvn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gzcmfcpog.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gravgkdif.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gmemmftpz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gezylgjkw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gxmjdhwns.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gvugdupfg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/grwqaevck.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gezoklquq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gslytycfc.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gselpzyno.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grukecvds.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gyzdpyrur.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gjonmfsqs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gntxpulvl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gokmitfoo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/ghwyjaacp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gasgciemy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gvloxavfj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gqfwcnczo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gartittam.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gcjydpdtj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gmtgesobh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gjknpvjrq.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/geqdsowog.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gwmdmnhbb.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gimlicwka.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gydukchjz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gcksooprz.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gbqqfcllt.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gibwtmjdj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/grwehsjyv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gautdtlpn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gxubufrix.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/grobjlaey.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gaxjguojm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gvkajfbrq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gixritqce.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gknnpbvfq.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gsykyrscr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/glqpifers.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gqvrpgexc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gncgltqgr.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gpzgltwlm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gazwpjtph.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkghtseu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gnllcvkhe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gvoqlscnk.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gtahqutbo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ghoqlaqoj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/ghsdzgvvr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gkjshpsjq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gruehffuj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gfscqsvxz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gmnttkqxu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gxqxtswhb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gcswigbrn.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gyydrjbez.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/glpocumzq.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gsmfwqzkp.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gavitebfh.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gzswtqnnc.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gddsvtavh.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gddnzdfow.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gdrypcfli.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gjbdpeedt.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/guxnakklb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/goaflumjw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gczsjsxfh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/godkeuziy.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gvedhtzdp.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gjaqchtgy.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gwodlfgkw.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gaoouxkdi.sHtML


<!-- 参考信息 -->