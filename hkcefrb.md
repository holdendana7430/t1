代发 wailian999

[B09] break 与 continue
来源：http://blog.fanxiaobao.xyz/Article/details/gvfwxtgpp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwdyffpe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppvvrxpn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdrkzrecn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gijexwkzq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gakwwcgsl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqhsgtqh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaxzoxjo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geemnikfr.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gabkhfpbp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fanxiaobao.xyz/Article/details/gktcrfowt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gahvnvorw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gffsmkjhw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fanxiaobao.xyz/Article/details/gcfwcpvqf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxssjqriy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fanxiaobao.xyz/Article/details/gntkzddmo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fanxiaobao.xyz/Article/details/ghnuyfllq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyrayudj.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqucxdyu.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fanxiaobao.xyz/Article/details/gysjccqhr.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gssvmjvhb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaausnwyy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmutactu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqybnwzvc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fanxiaobao.xyz/Article/details/gofeswulj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fanxiaobao.xyz/Article/details/greldkwpa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gxzbzdkzs.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdmhgblu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvjvccny.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fanxiaobao.xyz/Article/details/gwkapnlzw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gswwxhdzi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/ggkkokmjy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtxvnbaa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gujdsfjrz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fanxiaobao.xyz/Article/details/geuxipbvv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gregvbbkg.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmspjymfw.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsipljwn.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkczovbn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gicrdcsjh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gxictvwsv.sHtML

Java: x instanceof Number
来源：http://wap.fanxiaobao.xyz/Article/details/gdvbpvssp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlrdzhzi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgllnniu.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduarbyqe.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpsvqbhz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fanxiaobao.xyz/Article/details/gmzqhnqft.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fanxiaobao.xyz/Article/details/giuzszqmc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmahiaqp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gepdiblji.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gsxvgxppj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gouavflfk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfauptlmj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gylfakcmh.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fanxiaobao.xyz/Article/details/grllhvvxn.sHtML

Py:   a and b or not c
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvmrmdah.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fanxiaobao.xyz/Article/details/garrleceo.sHtML

JS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfvstvfw.sHtML

TS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfzywhvg.sHtML

Java: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gekclhevr.sHtML

Go:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnrjfkuu.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooyveuyd.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gknawuczx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwerlpqp.sHtML

Py:   if not data: return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpckzdnzw.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fanxiaobao.xyz/Article/details/gswvifata.sHtML

JS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbybidyeh.sHtML

TS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmunzigb.sHtML

Java: if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gshyfrcbb.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsjhgbfq.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpatmvuu.sHtML

C#:   if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/ghllrhxzm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goizusoow.sHtML

C. 函数与作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gpsfbdcxo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glrwrfnei.sHtML

[C01] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glzuuenlp.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaujuxqm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyftfdwg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goxmcvfmy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtvavyfux.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkoobwple.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkmhpjvr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fanxiaobao.xyz/Article/details/gwqojpfxn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvkhyfjf.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakjjgsqu.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fanxiaobao.xyz/Article/details/gwtwnolbh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzbulxotg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrtseoib.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnwkjfkhh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fanxiaobao.xyz/Article/details/gcaenshzh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwibupufp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fanxiaobao.xyz/Article/details/goeqnxmdu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcnrxepg.sHtML

[C03] 可变参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkivqxvy.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwewquwgw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdelpgtb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcochghk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/glkdnqrvo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwubxkwwn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvvkzbsm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fanxiaobao.xyz/Article/details/gigvqdrjf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fanxiaobao.xyz/Article/details/ggesbvpfr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fanxiaobao.xyz/Article/details/guvptxtfy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fanxiaobao.xyz/Article/details/galjxwfan.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gvbdxdofd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvgpambm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupjsoecp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrfcwyjs.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fanxiaobao.xyz/Article/details/glzmfrjqr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gdjdikgga.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlwfsfpv.sHtML

[C05] 返回多个值
来源：http://baike.fanxiaobao.xyz/Article/details/gzmmdazdi.sHtML

Py:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoqfyvre.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggacwdkij.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fanxiaobao.xyz/Article/details/gugysolfb.sHtML

TS:   return { a, b };
来源：http://blog.fanxiaobao.xyz/Article/details/gsjymfnvz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fanxiaobao.xyz/Article/details/gxbrzuehi.sHtML

Go:   return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gabbtarpn.sHtML

Ruby: return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphilceln.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubtsnisi.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gzygpcoiy.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fanxiaobao.xyz/Article/details/gcokdkfgn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpmauijt.sHtML

JS:   const square = x => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gwtxopwxr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gjjxggiuq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gqjnzttyp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gzifffwfb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjakyjvoo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gzawujdbr.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fanxiaobao.xyz/Article/details/gvqxokfue.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fanxiaobao.xyz/Article/details/gkhxttpks.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrltvmja.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvrzlmqh.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajmnkyyc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypphnxno.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlggxlle.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeutzllp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fanxiaobao.xyz/Article/details/gizdlnpla.sHtML

[C08] 闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzcawpsn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhekeapk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fanxiaobao.xyz/Article/details/grrwdgwkw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghezoqoza.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkndnlbbp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaihfngo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvxzuusy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fanxiaobao.xyz/Article/details/gxikxtilh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpsgfqnbm.sHtML

[C09] 递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gojroxzva.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxqqnasx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyvmpxfp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkjqyteo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gupkqllnu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/giiesahka.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbhspryv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyicdsvjh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbylrsxa.sHtML

[C10] 变量作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gucooeqxb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghasyqbsc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvlsiecl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvosyrvc.sHtML

TS:   同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gsrxncwvl.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqzdtgfw.sHtML

Go:   花括号块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gaugekbrg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/gsiwcksyn.sHtML

C#:   块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gccdlfumd.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrieeyiq.sHtML

Py:   from module import func
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqrbulql.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fanxiaobao.xyz/Article/details/gziwbqvtd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gdnjrqrru.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfbsufys.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbtznjkz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fanxiaobao.xyz/Article/details/gvfwtgfga.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpbflwqd.sHtML

C#:   using System.Text;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvadwuvlw.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fanxiaobao.xyz/Article/details/gfhwuenad.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fanxiaobao.xyz/Article/details/gdmxnizsl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxztotoe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fanxiaobao.xyz/Article/details/gojvxhant.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fanxiaobao.xyz/Article/details/gbebpseac.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fanxiaobao.xyz/Article/details/gocqxntqk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fanxiaobao.xyz/Article/details/gdmbxcoct.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbolpswm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkgxddctl.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fanxiaobao.xyz/Article/details/gxenjhlqx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gfwftiwmv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/grxaqxsvd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzujapih.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gysqhvcmt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphjzeony.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fanxiaobao.xyz/Article/details/glrjriyky.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guudtzduu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fanxiaobao.xyz/Article/details/gxozywtaf.sHtML

[C14] 泛型函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfmdbegqe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fanxiaobao.xyz/Article/details/gbtojzohb.sHtML

PHP:  // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfyqcfqq.sHtML

JS:   // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gwlttqmqy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdexwbcxl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gegthrgmf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fanxiaobao.xyz/Article/details/gqigqmjwv.sHtML

Ruby: # 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gtclgkmbi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fanxiaobao.xyz/Article/details/gpmrxmikv.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gytpxfwob.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fanxiaobao.xyz/Article/details/gacrsbiwo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganjrtinw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gsabzafsa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcbgkadx.sHtML

Java: // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwjcghxg.sHtML

Go:   // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gitsdtmzq.sHtML

Ruby: a, b = pair
来源：http://3g.fanxiaobao.xyz/Article/details/gszipdtzz.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiucwnke.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gisodrwxa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopixsbwf.sHtML

PHP:  // 无重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gfubgibhi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gryucioul.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fanxiaobao.xyz/Article/details/gblffopgn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzposyvbn.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgxfuvyc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfikxylm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjmnbqul.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwczmaew.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fanxiaobao.xyz/Article/details/gyliacvsy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpimytwzn.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gebmcbxft.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnxrfxkw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fanxiaobao.xyz/Article/details/gngkpioov.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbtwijjb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fanxiaobao.xyz/Article/details/gqewinhxg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtykqdagz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fanxiaobao.xyz/Article/details/gugqqhbxj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gluslbcsz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtluvsofp.sHtML

[D02] 追加元素到末尾
来源：http://baike.fanxiaobao.xyz/Article/details/gcpehgpwb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaekjgoqx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/guawqdfyj.sHtML

JS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gzcdvctic.sHtML

TS:   arr.push(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqzdikwd.sHtML

Java: list.add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbloefoza.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/glreaitrt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqytwctgc.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmtcrcab.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fanxiaobao.xyz/Article/details/gcgblbkwl.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhwoadjg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fanxiaobao.xyz/Article/details/gduagphlg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fanxiaobao.xyz/Article/details/gajxkoaue.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gxxzwjvwe.sHtML

Java: list.add(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwudvauzo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswnvszhq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvczbimuj.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/ggmdrehaa.sHtML

[D04] 删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubqpyyya.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gukqszufo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoiaorbr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fanxiaobao.xyz/Article/details/gaptqavth.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/genftcawe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuijegbd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsccysob.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtliyymjh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fanxiaobao.xyz/Article/details/gafrovcnx.sHtML

[D05] 访问与修改元素
来源：http://www.share.fanxiaobao.xyz/Article/details/grtkvnody.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjgwjiml.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gteqauhww.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gegbthmlh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fanxiaobao.xyz/Article/details/gjdwoicgc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guasssfip.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gtiserelt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gvudlgxmt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgmwkenp.sHtML

[D06] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/giwmucdgl.sHtML

Py:   len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdofgvjzi.sHtML

PHP:  count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfgeofej.sHtML

JS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbowydkpk.sHtML

TS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqauefuyh.sHtML

Java: list.size();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjvckxki.sHtML

Go:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gusdpayzt.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/grakaynkq.sHtML

C#:   list.Count;
来源：http://wap.fanxiaobao.xyz/Article/details/gbaptmzyf.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaidasdu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprcgczts.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gznyzcopt.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gyykrwbsm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdueayez.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/grvekakmh.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsncuqvun.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gariosqjx.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gckujyzct.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaknnwrn.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gjdtxceyv.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fanxiaobao.xyz/Article/details/grvwprvjy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fanxiaobao.xyz/Article/details/goewtzfcf.sHtML

TS:   [...a, ...b];
来源：http://blog.fanxiaobao.xyz/Article/details/grggqssqx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgeupioo.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkptgrqtb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gktpvadir.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/guitatxqw.sHtML

[D09] 排序（升序）
来源：http://baike.fanxiaobao.xyz/Article/details/gzuwuyrtb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrtbiryc.sHtML

PHP:  sort($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/grvodkorh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fanxiaobao.xyz/Article/details/gkklbpchc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwkmejsp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvejxmdk.sHtML


<!-- 参考信息 -->