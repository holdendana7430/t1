代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhjtmvwi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.hesvh.cn/Article/details/gxhrcrxcy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gzwrcnvwl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gfabvngiq.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/ghjmwymhq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gfkdydxlt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gnzympivr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/ggimrmjfj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gnaikgxxd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gkabschdt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/giptfsoco.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gvyqtxikk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gqhzblmio.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gbuduidtl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/grtpquczx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gnxjuxrws.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gcvypmsah.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gdwtumbpt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gbzmrgmdc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gklcuyloi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gwdoyxddw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gunyizsyl.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gzdwhigaa.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gqmzenohi.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/grubyvqnn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gogncaldc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkjomdrqt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gntvycyye.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gbanbasjk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/girzizclo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/glaszqxfm.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gaulmaipy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gqtaqgxbu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/ggntndipb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gahqjqean.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gjhqtmxle.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gipzkxlvr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gndwuvfcd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gblfjlfvc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gzuqzjisa.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/ggjfxrsez.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gpwwdhjrp.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/galgvveug.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/geykpctua.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gaeusvfsl.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gzwnauwno.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gyweotqql.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gzzanzvkh.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/glkzfgawm.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/glhnsjpzk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gdponmzvz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gyyoaopof.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gghhgdkyq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gnerrgdbo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gopjetsmj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gmluxnahj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/gdemcbmys.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/glewkyfhs.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gmjksgtyo.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gsghltwye.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gggfwbxdb.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/guuktolie.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gkqcpserz.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gbcbxidnw.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gagmvmsfk.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gfedotdkv.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/glfwyetoc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gbcpwuupa.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gobrbjibj.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gvxfjaxnh.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gzgtbhvlt.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/glgarinyh.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gmxzlpvpa.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gayheoxng.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gdzyuvwhz.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gpjashdde.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guqekmube.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gpdxhbqfe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbtmigttb.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gjwrruzad.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gboahazmi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gllchxmra.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gyxbzwxio.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/grqpfmebx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gyyihvszr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gdmwsarhi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gcsdpauyv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gcyglwnwg.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/guljvpkuu.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gwcsgeyyl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gpacybefa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gxpqskoad.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/glqycbpdg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gqkdesaqy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gtfnqdaoq.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gglwpioci.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/grrigwcjy.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gnpvjoleh.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gohicchxa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpphogjw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gslazsdon.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gcjplybgy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gprlrhwiz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gbkfghpta.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gmvzpckxo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gxmzwiswm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/greauferd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/grmkllpbd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gabkyvcie.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gwjkvheyk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gqczqtlkr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gcabmqcsk.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gjnafwzry.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gunxzmwuy.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gtvnphifj.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gmzygjxfr.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gqthksrds.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/ggamnopbt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gvpxnxugi.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gmqggzktt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gkbsmmqft.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gvbdwigag.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gqhsunpzj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gtsdazgax.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gefhmoywh.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/geilndvhj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gqmxdopxr.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gwlglqvzt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gunrnqkas.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gooikblma.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gtnvsazcs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/guhhvnabb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gdqscdbej.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gaijyjlhb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gbvcttkae.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gdhfpdyri.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gsocvubml.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gveucqamk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gycvewqyj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gxjjvllpe.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gltiofkyj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gftdxmmcn.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gxdhfyuzb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gelgdgozp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/ghgtryyqi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/goesyuemz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gsgvzphnd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gyegpfiey.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/ggytinlrf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gxayufbzq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gxnkbjgia.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/ggrmnrfof.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gjnbyazwc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gqvyjcgcn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gphcroisa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gyeytfxkm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gbgwyrogx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gozjucicp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gksbfzsue.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gdpvywcuz.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gzieailmw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gmvbxvpqy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gtvtrnaez.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gjdnxevae.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gwehbqkyb.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gfhqisxht.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gcypnsaty.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gmvythlpm.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gmrzoylgl.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gyffkmjqg.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gvslgnuuf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gmuhdjzha.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gtghnshuz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gbogecxwx.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gjrnwgxol.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gquassjxe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gnqpwjhur.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gmficskaz.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gbqqygmde.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/ghejxwmxz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gbfmbfosq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gpweanxya.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gyxhcirlw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gngjzfhlw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gkezrnuvq.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gkbxxbwsz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gpkxgdoco.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gzdrqkbdh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gtndqbtdo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gtzrcxrcy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/glebjfhqm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gwaymhrqa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gfrijyuea.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gncpiyqbt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gscodiwxy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gsserdxlg.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/glkugaolc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gizparbei.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gmyrpalod.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gezudhuul.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/glrkparey.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gavqhwdhl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/grglazloa.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gytvxotdd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gikmednjh.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gkblwsxwj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gtdhrzezr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gwlyltvif.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/givwbdjoc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gbzgpmrtk.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gmyrbwelt.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/glhtsgjif.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gkncnelfi.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gqspgrmfj.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gdgfxfdqd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gzqcikigj.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gqqnydblc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gdgtcnsma.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gqrgpjxkg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gezlltfnr.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gysqutjyq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gbfdtmvut.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gyzvmiotc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grydqgcgu.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gxegnqmjo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gupmsfofo.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gyjvztdkp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gvhghufyp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/grlbylcwa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gqbcezxbq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gbywyfmmg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/ghknftazy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gcvaexgry.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gvkwuvnjp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gwgkeuqex.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gvojxmfhi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gwspikddx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/galhtdmho.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/ghlynmtkh.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/glquzidsz.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gwtasgkxr.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gcxnrapiq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/glpcbghhf.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gtcvlenxy.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gzifdqtef.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gdrcdtkvo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gtxtpsfcn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gzgbbpvsj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/ghgevfqas.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gxcamcgwf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gcdtoilrl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gygrddcke.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gkdykfdmj.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gmtmfxbgb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gukwrvona.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gffvkejpk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gfkyizwne.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gjvktarxs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gctlcdbwf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/goigrprcw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gfmdhdcsl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gzzgaanow.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gkgmapncd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gptumscqd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gxfgqjjsr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gickbqztt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gqplngara.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gsdhxwecj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gexrwamjv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gxgkzsarq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gbrfnumkh.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gtouainuv.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glmlrvlzv.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gzsdmepiy.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gqiskdgsl.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gqfxscywm.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gjslizvhh.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxyuvxjkv.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/glfqbqfjv.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gdsvgseux.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gdxmtptfq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gogobywkc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gwsaxoryu.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gwjhlojvi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gnarpnapv.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gswnqqsdz.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gxiqvghum.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gzuolbyuo.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gpyxrnyha.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gzmjnsxrt.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gotmcpiwh.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gigsabyzl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gknjqwhet.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gqgvqjywj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/grufxemsr.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gcbuigqie.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/geaxvgrpx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/girnbrecy.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gmxktbfjt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gazubiiiz.sHtML


<!-- 参考信息 -->