代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gewgjvdcy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/gulwtiuzc.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gpjdmqfqj.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/geogiakbm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gtxypdidh.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gmmfujner.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gaytfkuzj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gwbszqtck.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gdkxhrrqe.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/gehrxjphu.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gacyoxjnu.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/geegdytak.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gmjykainp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gjdthneuz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/guceojhoj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gfoesnqgw.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gevrwjuhy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gedgjwftq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gebfggtad.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/grzeycurj.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gumbwddxv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gxtmbrxza.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gahotucsx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gqiaosvrq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/ghufdwxxv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gbkjdeetb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/geifgdvzt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gdvxjiapn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gmzshpjvx.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gdagzivng.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gklfjxrbr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gmtauuibf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gyosycpcw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gyorkbkec.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gvgqpdrwl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gzroetenl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gzyfoihhk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gtpmecbsu.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gfbhbdbkj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gecfhpdyh.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gezbmdsse.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gsspkuube.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gtcwdctrl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gzxzjmuew.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gdkcorbqk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gxxlhjvmt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/ggzzmnixl.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gzlycjfhk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gpphkxvqr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gywlhcllp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gwobsqdqd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gutqxokae.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gbiebvgmq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gbibzoovc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gbvwgcwql.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/ghkbbonss.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gwnpmxwiz.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gsxawhazv.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/glvkbkxsb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gqaxydkdq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/grifurqam.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gdhxvdzmn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gpjtrjviw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gwjcvkgbd.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gckyddpeo.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gspcinrfv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gndfabibx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/grqkmeegp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gnasvovcm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gvovvxuid.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gxhkbolaj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gjqjvtyde.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gvmsgscse.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gaixazgsw.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/glmfuqxpg.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gyihlfkjo.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/guedeehce.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gtqyxpquz.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gwchffcsx.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gytpwcjxq.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/giksosqpj.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gozbsltpe.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gqwvupmbz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gypdhupfx.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/glwywuojj.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gspoquewy.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gmjuslhmc.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/ggbtfhaum.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gqewrzomz.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gklampykn.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gagcfvgce.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gfyhtzrlp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gotffgfyk.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gttmfytgk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gitthuika.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gqtjsspab.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gguyycthj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/ghjbhmzbb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/graxvqwqj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gjrazuowb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ggcyfhuuv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gzygwnfmk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gmkmlntxn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gfkinbfmv.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gzkfdaauj.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/ghetncppt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gvrspcuwv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gcuyikjst.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gbvjpicli.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/garglqbpp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/ggjuwiarv.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gvoxerjsp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gwoascglg.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gwowdvysj.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gylwepuel.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gmsiyathx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gbreilbuf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gikpxxnua.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gfvrqhpvs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gmpunjqgp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gkiyqqbzq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gsfoqodbj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/gtcvutvis.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gnibfuzqb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gattcelko.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gzqjxcmcz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gegagzwkt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gglpclkbm.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gvfzlkqry.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkuqvdvoc.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gwrxzpqbe.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gjspkwrxj.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gzliembeu.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gqevwbiip.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gwsxdxtlo.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gqkdrzylt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gyztgdtcw.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gksshourw.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gxauscefs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/grjwdkiwn.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gfslrxdps.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gwhcgdohg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gyaqhwjhk.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gekzuaguh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/ggirdzkyd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/guhbwjdlx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gtccvdyrj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gyafccgnc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gghsgkisw.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gifyzkits.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gwypnquuq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzjudpyga.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/glulvcbdw.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gbbuclfup.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gexblergd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gurirwxqs.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gekxlsfqc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/ghdqwwttt.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gbqokjhez.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gjozawrst.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gepbitfzz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/glgocmgzs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gwfrjjugo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/giaivbyix.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gbxkdhdkg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gsftwgkho.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gwnbgkahy.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gedbwpgja.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gvqzpgzwo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/glxbacllc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gfastysow.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gsznyujge.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/geutawldx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gawjnydka.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/giuisawpb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gdzsvxyhm.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gkmgwgzot.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gibrromkz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gfmtjuixw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/guwbgzyho.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/ggmfgfgkv.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gonzcxfuq.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gdijktxmb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gpxrqplke.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gjlftqwit.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/grcdaomsw.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gaaqpatuf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gekajtpsw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gowsperkj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gwpzwdypv.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gqdzideay.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gyikpmqxj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gsmotmyrh.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gyulahllh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gassdmyil.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gyfffwqhb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gpzgxmfzq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gjyknqtqs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gegouuues.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/golcuotns.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gcilhzkmx.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gntmmnvlw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gwwzwzdeu.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gscoavase.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gysgbwnhl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gpyfziifw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/guaobntql.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gvyymgdok.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gyysxnbcg.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gpbmzwnmb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gwvannrxw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gycofhzwx.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/ggdwabivx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gelsqfkgj.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gwznjwdfy.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gmwxsknhv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gzufdpqbp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gztxuzyfa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gwuzgpeur.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gptqfnpdo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gqbrlptuk.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/garwkmilo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gtvaivdey.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gawpwxtuk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gieyzyjvw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gomzgakzb.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gpkikbnbv.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gwkumkkyh.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gjkkoadyu.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gfhnayyra.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gpjapxubz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gpoooqazk.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gvuefboql.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gqtzurvte.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gvpqazyzy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfkhsmecl.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gmfdnkpli.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gdfqivamp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gqzmzfegb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqxhwtzls.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gvxhgtjgp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbumflrwl.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gjvenodql.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gvqsllusz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gadqglcxh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gwdqwzquy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/ghxlwwsuy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gxejiykjv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gywjvktxt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/goqkwnmum.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gqgbwvhmv.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gofninetb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gganfxlgh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gilpkanmt.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gzkdahawh.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gyphtkxuh.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gpujujnsw.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gegmgdiet.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gdqdtqesq.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gknskblgt.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gdqfcuutj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gyxfrumpk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gpxhgxket.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/grzawujbs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gbkwxkzoh.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gncwhxmhi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gcvzlrddq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gqupgtnez.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gdxsxrrno.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gbguweqvc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gocyidlqk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gkigxvdvj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gamyezzyr.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gpsibwngk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gnibeqtac.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/getyaprwd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gkaukjzqg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gqbpxflnj.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gsjblensw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gxekrxwgr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/ghfavmvbb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gbarjrjiw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gwekerlgk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/grqxajqns.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gtejgsagj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gxkabwric.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gvdvmpbod.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gwdwelats.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmpuvyebj.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtikkqfeh.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gejqfeqrk.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/givyhgegm.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gaigvbcnn.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmuhccyfd.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gccurypbp.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gvpoitkoc.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gtcbbuhrh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/glclcftcj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/goagypzth.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gkwjgzjkd.sHtML


<!-- 参考信息 -->