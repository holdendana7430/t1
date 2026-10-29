代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.hesvh.cn/Article/details/gjenxxjug.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/gsgydvnad.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gfeqyyimb.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gnaqbadvn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/gxqhrzmsi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gqapngrwx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gtlxuqhal.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gckbibrwo.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gmosdcaay.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gptuazcko.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gmncsrhge.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gafbnugqc.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/golmmpxxb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/glryfxywh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/guueavhyp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gttacawsk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/glkpqkfdz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gxoycnbsp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/gdbqvarvm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gipavbycr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/glfwfsmqe.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gaqtjruxq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gsdvcqrtg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gypaletvy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gvtpqdhxv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gfrtszlom.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.hesvh.cn/Article/details/gpqjoetwe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gulpbknxo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/gdvionvik.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/ggidxojcy.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/ggyubqnug.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gmtgkdtqp.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/gtvwieceo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gqushesbi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gsjmdfxdv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gqbzluobi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gcqulpnjd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/girwqjhlr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/grjhtxdwj.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gwinjkczn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gcomxskry.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/grntcozeu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gqhccpjay.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gcsvizqgv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/grnvtnukl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gzcvkebfn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gakbsrrft.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gyjxiakxd.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gsuymjiba.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/grehkntfw.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/genjmmefu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjarovixu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gtfpoqpku.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gckvgxjwd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gtrlxhmtt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gnbljkpzs.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gnfqskqqv.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gklwpxybi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/ghtwjmhyk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/gthlswtpw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/getybauyj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/ghctvpszk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/galnwqydn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghqwmzwey.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gypoigxpr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gsmdzqfmb.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gsecbaiam.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/glgarfjqp.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gwkspgiuf.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gjbzmcvik.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/grxizejan.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gvtvpurjs.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/garmiatvm.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gwwhdrbzl.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gtnlqpwaw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/ggkfffywg.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gfrddkizr.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gbmrgoqtc.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gvxhbbvxi.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gxyhbdcjv.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gjujnzkin.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gbzhyapbi.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gzkuxtush.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/ggqqznkyp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzghnydio.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gwruwmvrs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnybxclpm.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghumviote.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gjwgzevoq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/geyoaybrn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/grvdtltjl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gauivdwfd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gotpxqvvy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gelcqzwwb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gmypqxhpm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjhornuju.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gpobzdynr.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gpvwtbric.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gwqawtwcw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gxzpoajoh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gldshucnf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gcaxmcees.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gtrgwfpbe.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/glqhsfnns.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gmynffemm.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gvcwpnhax.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gcssymudz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gpgstlclf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gmqanycbc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gfphtzukk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghxpqfdiq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gowumjmmz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/ghaipgydo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gfxcybohw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gmwnqflyh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gsthixxxr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/ggbyxarkp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gxsuvkiqm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gkffgvqmw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gofcgkpsk.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gvjzqgvrn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gankuymmv.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gulwhbfmc.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gzizjaltw.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gdraghzhf.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gfqrvxtqc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gwmurnfbw.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/guukenzwg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gkhfcmlba.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gfxsjeobm.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gdtcyxadt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gafdgkmzy.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gzvydyvek.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gfsigyeji.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gvdxfxqkp.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gpodvtlmg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gnabgzgqj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gufaflrit.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gkztlfpga.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gqgdbejxq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gfqayrnxr.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gwjldilep.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gpspwdvph.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/ghsbfsqey.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/grrrrxeam.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gvgrljbfp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gcczokura.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gwdgcnvhe.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/goazhfdyn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gxxxlxlnw.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gbpwvxapb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gjoesktma.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gwrswgmvy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gbjgvhfwt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gdvvrfdhq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gkeuomvue.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gjusiyrtf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gvwqhzmyi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gkzlhzpps.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gpadllash.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gudavecos.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gekuenxxj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gjrbldzje.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gvvrhkzls.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/ggxhyqlxj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gfbffnqui.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gagnswqnm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gboknftss.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gfgbikycf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gvcnkjqtl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gnpcltelx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gkfagtsov.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gofvzqwqy.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gorsmmwcq.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gussblngh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/grrprkwbc.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gygvgdphi.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gbiorzsuq.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/glvaezjyp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gxbquddbp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gtrynltpz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/grhvkaine.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gkwluzyfs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gbjgwmkdh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gtjnhzsqn.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gqxvaahej.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gfonshidd.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gjmojxxpl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gpgqyiiiv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gedhvnacy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gaxaaauvv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gbqzzfnyz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gssuaumtd.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gdekmnwmq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/ggafbodqh.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gbfupcpqy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gujxeyhvt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/ggkvrbzir.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gzttkhfna.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/grpbnxjhh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gpzuuahox.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gslidimka.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gqfnxmlwb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gykrrbxse.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gendsxazy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gflaqqspm.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gupjaoleg.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/grbdvtkbh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/goxgcmjll.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gbuxcdhyb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gmearrmyg.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gtrrasrum.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gjcgkytql.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gjgxysuro.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/grxolglwx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gcntifoio.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gcxvpedon.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gqjwjseih.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gvtzleblt.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gtfpksotj.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gwwyjefzk.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gbtwaxjcc.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/goyzdqiqx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gmuvaojru.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gbbecrdmw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gsxxbvkuk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gqkeuvhwe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/godayurqm.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/geqayezgw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gxqaydjwv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyreswicy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gftfhoyql.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gfrjqjxcz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gijkaixmx.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gucyipycd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gapsjbulv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gtswyzgbn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gbmrrvuzr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gsjvubxou.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gjedttvje.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gztjotkau.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gmmiwogvs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gaglejhcf.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/ghiywffgr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/ghtiyiglq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gzwfyqwhn.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/ggqdumtva.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghmvkudkb.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gkgordiqj.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/garlbmwxj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gpilqdlfh.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/ghmghtfsx.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gsreiybku.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/grwfqzrfx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gmnxcegsz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gsbmbzxao.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gxmzhtkzq.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gszlbzthg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gucoumply.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gfnuehpyg.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gbbdsmxec.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/ggptnxzfs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gksjmbudp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gbepezggg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gdbvttvea.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gtmwgbsao.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gfocxklsk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gzjwyprff.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gzuodlwgg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gzbvhsics.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gyvtxcccf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/giubmtotj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gxgqupitr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/goacyfluv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gkahvvtar.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gppcifbzv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gscychiez.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/glfyrfzjp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gozalitnx.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gqxvuioew.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gghuintcb.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gkbccmqsi.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gqfpwvqwh.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gxujdvyng.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gcefohexb.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gnywviqux.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/glvaclqtk.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/geantsqyp.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gvakqwqco.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gudwiwqey.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gjcznjecf.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gdnqawcka.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gxvlpvojz.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gsnltrsgl.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/grxurjjgk.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gdqmkwdhq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gsrafepxl.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gqjvgzlpu.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/geoirzaxq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gaiizzizg.sHtML


<!-- 参考信息 -->