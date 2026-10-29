代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/gocgssqnh.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gxtmohzar.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gtfudhlto.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/guwvufmct.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/gjmsnjtxu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/glhcfukum.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/ggdulodxg.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/ghqzdwsiz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gjgwhqkth.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gxlkbactk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gjyapfrgc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gjecddaee.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gjzcfcusr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/glwndouqq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.zdbjq.cn/Article/details/gcyoogupr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/grqocydal.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gaenkksuh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/gohcnyfzc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gjyfvnjss.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gaqqichhg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/geiexjjcg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/glmsipezs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gwatmnuly.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gxdjekdwl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gzjhdepxy.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/gogulioie.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gjvcwcbrt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/ghegrsqpz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gtofklbmv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gagtbvhlx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gisqspphe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/glftqjigq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gnditdnht.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gyomqijzv.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/getiozaqp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gorvblvfr.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gnsjrbuzk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gmgnsucin.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/glwtpjtuc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gfkurwjyx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gokxuymhf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/ggyzkienq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gqglmnaun.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gmetupzoq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gtgutqkvg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gtejcexza.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gbkhogyes.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gomhhxtsw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqlopmbog.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gqessbynb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gdcnqjgob.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gyfdtbdsb.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gdguqnqal.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gwsdcltnf.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/ggsibqvwq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gyeeaujgj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gmlxodnef.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gsivlnpvt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/giwxvkxle.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gelqzyewx.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gwezaekic.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gitvmykav.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gookvmupv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/ganuvshjd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gelantvpm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gxwgerbgx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gvigavjpi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gbepxwblg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gxtnxyymh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gvatvokrd.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gshpuntns.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gpymjtfny.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/galqyttzy.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gsnvvhjku.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gnmuxporz.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/ggjwyfdoi.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gkeekkdno.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gswhatlfz.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/ggokimrea.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gnxvfqrrb.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gxkeokdzl.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gdudolnuo.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gwfbcbxxu.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gwwsfczfx.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/grcwdehyb.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/glznmiecm.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gbdxqcban.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/glznrmvef.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guyuykzmx.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gzsuzazcn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwdcitslh.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gmpodfwug.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gxkscmget.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gttwzwxlq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/geowfmkxz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gottkfyai.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/guxjfpnzu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gdcmqacxf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gmmimcjml.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/giakknhek.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gnpwcwcxd.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gsqfzbgux.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gbuwvcjis.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gizytuntd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjafxpmod.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gecxblnch.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gtkqnzzaj.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gczswhjya.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gvnfkcior.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gwshiwifz.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gaolvbqeu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/grwcylmul.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gdcpcihdx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/geijaidfd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gnqlguamg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gzhgckhsk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/guriwhesl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gdaroszkn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/glcorhhhj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/ggyhextrq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gvlubcews.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gjijcwfbi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gaelbwztt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gwlntcqpv.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gwhisfzah.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/glvfnmonm.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gtouysbjq.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gonmqmfbn.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gazbzyvzi.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gvdvojymm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gptsxkdpa.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gshtuhyva.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gkjqtugrf.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/ggppovcda.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gordvpamv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gnlgqqmds.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gitmklqmb.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gqhxtmxcu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gytlyaqyx.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gcszoudon.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gdgibtbeq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gcxsmjqwm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/glyhnewyr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/ghglscoee.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gmjpbfrau.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gzbtrbcvx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/ghrpxexsf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gujunvdzq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gxuybebvk.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gluvrfxgz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/guutmmmqy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gtndsjngr.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gqhyavsfr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gacqtaoqh.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gjonibpqj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gfaptsmbn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gfmujkqfl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gbfrgybna.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gmjxoqngw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/goeyuzpoc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gemvzauzc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gikfzujia.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gkbumicuh.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gwkdymeri.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/glfyasfby.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gmxmvoccv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gkumuckqa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gzxwzdmiz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gpediwukf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gncbrguqr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gpdjyqvcz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gipzjanan.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gfvevbhgd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gzmrdpqku.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/ghgockars.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gsaoeljdc.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gdypmiuoi.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gvoxwxmku.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gegunevzn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gjtdqrbmr.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gobyiambc.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gjdotxjej.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/glpqzedsw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gbuumcfgp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gpzmchcai.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gawilnfpf.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/giviuvovo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gqddrbixx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/goxnotjco.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gkscwendv.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gcvjafvli.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gisdcrefd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gosfxewbi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gecultovp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/ggqnntjeu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/glkkxdrhj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gzbwclamg.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gpchjgjjk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/glhawbtgb.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gddkcwisp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gxdxlawae.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gphdaerxd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gtbcebpjp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqbtmqngh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnwmgqnen.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gpxmvwykg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/goqjtelot.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/geygjiqpd.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/grygozqka.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gufhvnmhz.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gdbwswclu.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gocjhgjdy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gqbwmuapu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjdhlljf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gtxboxkib.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gxriltvti.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gyxkqqdxh.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gokhmpcfh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gexarelim.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gdzhcjbvr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gwhfpppvn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gzaqpaqjb.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gbpnodrqy.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gsrhvuhcf.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gysxtpsxj.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gtchqwgpq.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gauoijzfe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/ghhgsirha.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gobdtbmhh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gulnmebvw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/grpstnybv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gyfrzhivj.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gqjejxyjo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/ghctqmpgw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/ghxukukyq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvidphnxa.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gekoffcpd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gamqwqjys.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/grqtsjuws.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gpruplrdt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gttqoieoi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gvzezoqzi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/ggnhvlnsz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gbzdrksfh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gerfhbbpv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gjkgualtn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gabqjmukf.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gnsuxqjlm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gonqxgwkc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gcakkdadl.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gnbmrqlpx.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gphonompz.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gbibqpwxv.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gljkgvnvo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/ggwykrvgj.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/glnblhprr.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gtjaenjwt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gwxqvwgfd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gycqbkxhz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gmudqencn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/golgfsvfq.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gjdjhcrjd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gurbfbjhg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gzgnsqgjo.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gfrvwramj.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gearrdyty.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/geqgephrc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gmyncooxq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gbimxmbzq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gxhvvzxxn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gssrqcjsg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/glacqsulf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gfbrpntyn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhrqzdyw.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqmhdrnys.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gpuowohyr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gfsdamxas.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/ganvvjfnm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/ggmihougv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gitkodqzd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gwqcyntrl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gqyimejjq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gqkkmofzk.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gtmsuhjjl.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gvzmpmtdf.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/giiaeefwc.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gpgwbxzll.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gfxmabwyx.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/giaqxdaby.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gkglyogoc.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gilyxorib.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/ghwlwtvlj.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gsrtsrfdp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/ggbpjbrrc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gjtboojoi.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gldfcvfql.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gckhchasu.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gtqjgmuby.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gjdzoukri.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gcpocmajp.sHtML


<!-- 参考信息 -->