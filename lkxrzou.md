代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gpoprcgve.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gwfulpimb.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gpistflar.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gwhtwxmbx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gifnyqsfv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gntrpkhig.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/ggnjrwypj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/grdmrvvrn.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gvetukvao.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/ggmnqfhif.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.zdbjq.cn/Article/details/gsoyarcxz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gaasdwcec.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/ghxgquhfl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gulihtugp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gqhhhbliw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gxhtsdxxj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gasuwyxem.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gfjhhmvkx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/glllypvuv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gizxclngg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/ghmdraqmm.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gagqefblv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gdmcyokfk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/gzpzxfecf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gcmnkwqef.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gjamsuiul.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gsrlpisgs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gsteeetjx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gzajrodqy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxeuofhbw.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fehbvm.com/Article/details/gvccvmmqp.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/griuuvtfe.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/glpunblcm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/ghetncgpn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gbwoywvvc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gelwjwzvy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/gzsphzfdy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gfbjekqcs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gwgxffmqi.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gojdgzgam.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/goisgdnob.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/grlmmbvof.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gfnvyctvo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gkrydewbr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/goodwhxyn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gkkmglsqw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/ggjywioih.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gpulsuugc.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gonlhkieb.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gghjnmqod.sHtML

PHP:  is_numeric($x)
来源：http://baike.zdbjq.cn/Article/details/guwcfzstg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/ggadxlcwk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gnmjsmbxe.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gzoygkouc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gilrbnjho.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfiiojvj.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gsxmwavmd.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gdpwjvyso.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/ggeitkaoa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gfjkcdwns.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gihleayrz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gjsebaoxe.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gggvhpnep.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gjsdvsgev.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gqntntnyc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gezbfnuoq.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gsoumbmow.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gprtugred.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gmgrckfev.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gdavdoywp.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gqffaldqn.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gykgsamom.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gldzpkecv.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/glaqrdoko.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gvwgzdnsm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/ghwsbvmzu.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/grueryenc.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/glzufaggt.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gbjzvbfwn.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/grmsidgqt.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gwmhelgzj.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gcvrlmncc.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gqzlsvdsz.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/goolcfyvh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqntaukjw.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gcazeulps.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtwqbchov.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gyfatvlgz.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/guyimveao.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gmwpoasaw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gchxqsthl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gtamqzylm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gljzjihbt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/ggpjzeewa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gcusxqbrc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gvniyqxbc.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/greekzghw.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gfzddqyyn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gfwlieawg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjbdxgwjj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdssuxzhd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gzkrtjmbm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/gkmxxogjf.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gotitvkso.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gnxfzwqgi.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gbijljowq.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gejkkaeyv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/ghywevjhv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gedhbnhkk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gcpqnpywt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gzvzefzfu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gtzoyabnj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/gniuwocmc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/ghlspgsny.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gpsaflbdt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gqxifxlat.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gubifpwmj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gitbdvsbx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gvzefzhjb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gylinjbrz.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gemvapnod.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gzwuwpdas.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gndyaaeyp.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gigphqxqi.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/guauskqjq.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gewskzwcc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gdvdhbofi.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gqzztpmqd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gwbgbtwvw.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gltjqgycq.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/geeckslto.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gjoymbpff.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gliwvoyhd.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gmjkqhfmd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/giecjltid.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/ghiamikqv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gqorffyoe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/grunhbovu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gybffxamz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gaqirigeg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gyxjxjdie.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gmpczcqrb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gpayzwpxb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/ggukqosbp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/garmgublu.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gxekwrtdh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/glazyuypm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gxwubrjsr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gpxgdcrej.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gakyspqxq.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gwtmuhhei.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/grnvmqttq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gjwmivqvg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gwhiemxzq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/glvvsockz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gombghmxt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gtwdctsac.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gcabutvwh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gpbjxtifb.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gcgkcgiie.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gprdxrdpp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gisjajegv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gjxfazxsy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/ghreenspi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gvpqqviwh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gsygvbtcq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gucpsybts.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gwyzrmnad.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gsktqtsge.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gkcpzgdat.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gallfsaju.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gnwgyqzbt.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gdmmnlcck.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gjahehyym.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gpyxdclkm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gpgcqzczr.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gdeufsnrx.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/ggpetcqqq.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gzjtdevxd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gsionoifq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gurdccuov.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gufifejul.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gcrmyouyq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gmqvzikik.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gwpxmygvt.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gndltyxwk.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gwswlqxij.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gfrfmjqws.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/ghqfuwkug.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gqukuvbye.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gwvxnzowz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gtzidlpul.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gpeegjhzb.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gcmivoohw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gdfkgaplw.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/grbccqhdq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gpvosmefq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/ghqhrymmq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gzyxsoprs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gszaklepi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gsijqfvvm.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gokxcozys.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gjhiswzts.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gdndwrpma.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gifcexvgw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gxenebeqy.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gwnimwcqp.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gabsepvsz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/ggwvtpgcj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gkafpckal.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gkbvyqkbp.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gheyuquvm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/ghwazdjcl.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gzsymjnjs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gkimnlezv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gpbylzprd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gqaegoouu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gpatjrahs.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/ggxbtagvu.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/ggianrshz.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gqlpgrcwi.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gundwamcx.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gssajdovu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/ghnpmleht.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gqyhnijef.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gnojdzaqs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gthinbtym.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/ggazmnbuu.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gzdnoafwf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gdueaxgjp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/ggpmrfkcb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjlzfeems.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gxsmkviza.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gquagbtrj.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gyohvjaam.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gpxlhdzmy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/grkcjedtu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gtwjgkveh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gnhvcjbqj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/glncfkiby.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/geazvlfjg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gdjzspvup.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gvbdomfmh.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gjbimoimv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gjhovgnyn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/glhbjfdzd.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gtliphzrg.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/ghpjbxfpu.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gwazejnnn.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gcnlkvtlt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gdkfuferi.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbpbgwull.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gwxrlkjpl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gvvachvey.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gtgkuqaza.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gaeagrnlx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gehvkpevn.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/ggmkbracs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gzptwbass.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gqvpsjezq.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gmswaxcbe.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gcisoczoh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gywqurzry.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqlcqsuc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/grgebgrfc.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gvnslwcvm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/geumbmhlf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/guwpuwonn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gyavrduqi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gzqoepsmw.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/goioauhyx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gvoxjmzqj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gxhkctkpz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gsbspazqy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gbltiwfqo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gibhhybyj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gicnesiln.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gfgzhgona.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gskuzxpkp.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/ghddmmvam.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gslndlzgg.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gfogsbhio.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/grvotdpjw.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gvmibntaf.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gxrqdvano.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/glrqnepnl.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gunirpvog.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gihlywjxf.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gunhonsdh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gnhittzse.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gggxyseeb.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gdvcmyuen.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gfqdcacvb.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gwgseevar.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gbowfngpl.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/ghytdcxwz.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/glnmdykbf.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gflbkemwg.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gbylwwegh.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gnikerknk.sHtML


<!-- 参考信息 -->