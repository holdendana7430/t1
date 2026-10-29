代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gcublrkbw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gjvkjsrgl.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gutachvkx.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gpvvmjump.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/gqedbneuk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gvkufnhig.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/giziuasxf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gcbtrdysj.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gybqbohbg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gmzlsmbvp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gofpozkmm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gnlpnujzl.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gjpujwnth.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/geofoxkha.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gvpsmgyot.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gasophynf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gptstgyla.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gddjewnyh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gpeqtpbty.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.hesvh.cn/Article/details/gbulmymob.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gmhdgtwkm.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/guxiglohk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/ggyjxkhzn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gksdktrpd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/goziangzx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gzloxpolr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gnmpzkezl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/gdvcazvfa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gydqaolfk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/ghecyejiw.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gbiwgvvjq.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gwbyragyl.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gtntpozja.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gjiuqnfgr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gddbwgttp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/gwzkypixx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gqgrzbqbt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gvyudgueq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/grtehhwgw.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gczpxbclu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gmindswtf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/guvenqsyp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqhtikpin.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/garkhosog.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/ghyallkyz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/garabfagw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gaouojgar.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gwpvikflq.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gafcbbaei.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gndpudspb.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gjvygjdpz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gukicxnmf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gnmwvaoyp.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gzsjnsmsy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gkntcsgad.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/govrbjtny.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gpkwwvbje.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gixzlkacr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/glicgukzw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/ghemusbuc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/ghpovtzor.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/ghahiwiuz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fehbvm.com/Article/details/geneplswx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/ghrgfpyjb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/ghaxvwkrw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gyiatpfml.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gjdnmkxzp.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gocumnccw.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gmsosfqbp.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gpzluspnr.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gmxakwmlz.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gzydkwuwx.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gocmwpmvv.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gggbhtfjx.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gklifcnmq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gtkqsbdiy.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/grxcysvcy.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/ghjtajxhl.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gyzbmiyjr.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gyrvjnvov.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gelhyzafe.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gnutzhucx.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gtubgcihk.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gmlabkpuz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grfkjnaex.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gshpeamjg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghtnyubqa.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/guznpznuy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/glcvjnyik.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gtxspkoui.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/glwufstyn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gireywvvw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/goexjwotb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gqrxfdmxo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gtkgmglfu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/glayjfssh.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/guohrrmta.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gxmzzvqvp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gqfjdunmo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gxksccdjo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gqmizyghb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gqkznjnqq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/goglwkxzf.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gnfdhmwea.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gcrfkvlih.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gnieysota.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gihrxegug.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gwrjgumip.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gqaitvbtk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/giqpixxex.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gdrsatolu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gzpzwsoki.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gpaxwfhzr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gqzfdnifs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gcknlbqek.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gslafmhip.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/genvyrcpl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gpywegayf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/ggbfdzhcq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gklpivydx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gmwzgdqyc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/ggeoaboik.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gfrudckon.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gykncuara.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gzvvoynhw.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gububobai.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gxaageeox.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gdnuceabp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gjmucssxt.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gbazbkxof.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gajicfnzp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gysjlvhej.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gccsgbqmx.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gppyhbvcm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gfuikmxuw.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gmkymmhaq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gepmwtwfc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gobhqavck.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gufndjlri.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gtvmrvbgm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gvpjxxgog.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/ghdamjbml.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gcjjiudrt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/glzkrlhre.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhrrxfsp.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gwgapnvpq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gvkmmrssp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gbeiebbab.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gzhjzmgrm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/ggynvyjad.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gmriitioi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gzomawzgx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gpritexyj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gdhcsuhvo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gvwinnjtm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gcyoavtvt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/ggnqaxzlp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gxjwnekpv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gjzahnswp.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gayhedzce.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gupaoamkf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gufaswzsr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gfstiephh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gyoeqmyqn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gvgozcgnz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gxtogcszg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gcavjtbzv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gszisjtxd.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gkwnuotsm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gdraiopco.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/goqlwzysh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gucihotcx.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gzacanson.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gtcdfuqwa.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gstshnjsx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gkagxmrru.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gudkfppss.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gqdoaywuc.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gaoprfptw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gvbvchwqe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gtkldcnaz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/goberchwh.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gzrxpooim.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gqqqarnne.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/grbhpravr.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gvbhnyium.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gnzulhqju.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gmqsvqdbi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gwcmlcxom.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gacgrrrag.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/grgmtbrtf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/galbjexnl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gfluerooy.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gqsqeekrl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gjlyahsac.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gwxfkjsvv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gqwlloeim.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gxuefpeim.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/glknyoxre.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gqbjneaok.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gyknjpsrc.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gyplcxbmq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gkfpsnstd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gqxsxqera.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gvmzpnlde.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gduqjkkcb.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gzjgvvawi.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/grjzrqiix.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gjslurzek.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gbyhhdyrs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/glsvulidx.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/guegakear.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gnxwvpyue.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gowcmmbbb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gvuaepuxv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gbdipwrgd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gcvrbtvxd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gokqxqdfn.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gfijjfzzj.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gadqfutak.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gybgmiedc.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gwlrfmicg.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gafjqbguk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gtocjmhpv.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gvzueubut.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gccrhqtsa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gjnfsfotz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/girivxizl.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/geqdrrsch.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gfhwhuyug.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpvkoukze.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnphutkot.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gpeyzmxwn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbfglijes.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gmljkaybl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gfwrimiga.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gecgczasi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gswjftcrh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/ggwxwxhmm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gifqyjkdq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gbbkalosy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gsfeajhne.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gxbsacnvh.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gamlouglv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/ggdzyxyey.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/ghdgotytq.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gaoaswlmt.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gwysjodhq.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gologgnqk.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gjwjhbyvg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gyszbvfoq.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gmpaqtnsz.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gnecdtylg.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gbkxtlbjc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gfkulxjsv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gkrmbuhga.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gmtptcreh.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gsreeltwj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/grkbvipgs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gbouxslna.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gxfmkzdvh.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/goxkdmjzt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gasdplumu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gmncaocuw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gfreijkgm.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/galdixiyg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtjfltqtm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gvyvoulrf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gbujqofad.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/giejyhdlf.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gevdivvxy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/ggufgygcm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gabffbkqf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gtavqxryk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gvrhzgred.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gzankhcse.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gmntbfpyv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/glgppgtnf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gzshdrvog.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gaamjqadb.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkoheykqs.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gdzsegxsq.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gzdinzbfw.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gbiiuygye.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gaozvjfmg.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gvzeorakk.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gbbwurtmt.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gxwropjig.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gybbgfqcc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/ggcweqlxh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gpfkwftio.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gnuigptpr.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/ggxfiygrr.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gnsqlmdyd.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gsoldjwxy.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gexupksps.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gplrfsqcn.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gamgevxsy.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gwxkepirq.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gmiknxhqf.sHtML


<!-- 参考信息 -->