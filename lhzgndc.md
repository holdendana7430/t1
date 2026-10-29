代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/ghldlscnp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/guwijezwp.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gdssoebvb.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gcwvppmjk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/ggprstmuv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gkdqmoywt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gyfgcnezi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gnhqpazug.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gqicisugw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/gxkzpwptf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.zdbjq.cn/Article/details/gfrgmxjvt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/geodnmcmi.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gjolxtjlq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gswlgerea.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gfnibqath.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gxqqifdyv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/geqwkvomz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gvvqslfyr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gksccmihx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gakbjupex.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gskoadsup.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/giqgnbuyg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gklkrwxse.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gmycnstip.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/guwpnvjpl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gmmmfpyih.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gvtidyahk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gzekutzig.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gjbmyaxqu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gjsboimpn.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gmjevvizv.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gpuppkypu.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gqybmwyfx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gebfdbnmv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gpyuhewxu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gzswcbnum.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gsaswpwek.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/goideuqtc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gglnvjenp.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gztmvehcc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/gxjkrbzvc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/ghuryluog.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gbwvcnlsb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gboigclgt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gndgtgqqj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/ggqqraocx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gcpygkhkf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gjmnztjzo.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gitoqqfeu.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gvwmotksa.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gmdfyshxo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbtfkukuv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gonmmksvq.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gnztmnsjl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gagyyucoy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gujiyamjw.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gnizaswxd.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gmkehroip.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gusyihzvj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gxnzjxupg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gkhyfdjop.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/ggkrhookn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gajmblknh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gdpcfidrd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gopmcnlwh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gftkjhtxg.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/ghgkrksfo.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gexkcluku.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/gdbfzbblr.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gjecherqi.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/glcznfaqx.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gcllvswrk.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/ghhjmtyun.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ghugtrwnc.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gfzmsiyxe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gfhewtowd.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gemeurfjr.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gzlbmjuoh.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gsrfxxibj.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gdktsvrnk.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/grbchltbg.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gcwgqeoys.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/glfwxqgcy.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gypbnmhug.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjdgseuos.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gmdarntfe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqpyipvrj.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gwnebnjqz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gspeavilt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gclaajjif.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gkkdgragb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gglitmgav.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ggklxhtnb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gnflzetcq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gsojwdybm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gabrguyiw.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/guthnobun.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gaumbnzzf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gxekdadds.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gwtyrklch.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gjwpphcpm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gpahomlxs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gsdistiag.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/ggzyurugk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gzirngfsa.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gbgfvigkd.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gejetgtnz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gsajzpqxf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gccmgndsn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/grvqjffkf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gmqyducse.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gikkbcyrn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gbethnuaf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gsudortai.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gkhbizabd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/ggczjcyss.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gebbrmiue.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gjlzsjkkt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gmwsdneia.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gnpmbxiyw.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gyimkxvnj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gyhmpnodv.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gdpklfghy.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/godqljugp.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gnxhooiaj.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gqsnhhsva.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gzmjxdvwz.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gamitloqf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gnuvtmxrn.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gbalmwuwz.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gqwyjzwgh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gvylxztlr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gkydydqfp.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gzloijjwp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/girutvtmm.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gkyqvyety.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gxudyzpql.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gxifxktde.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/ghqtuzfqd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gbqpnfmdm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gjsutexbs.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gdblvydsk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gsyvntzsl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gtugvcvrn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/guktopowz.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gzrlwvfuc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gjfoyqiat.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gkkbvajco.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/ghdvuakul.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gkscjwhzf.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gcwhijghn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gvguurkry.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gpwefnlum.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gekjegjxv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gsxvkssen.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gkgwoxmtx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gvlmtimoc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gruwtetwc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gyumdwwzc.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gzvlyjfll.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gysscsmgy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gozipkgzl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gxkdjuiru.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/giuoojvsu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/ghqxgldcm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gygvvyoyr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gwkgcxqtw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdhlrcku.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/glsizynzv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/ggcijsejj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gpwwqhtit.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/girbdvvey.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gwtvyuvrg.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gicbbgcrh.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gcoshadlp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gsbjqghgt.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gkehjfmrx.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gehjvyhwu.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gyboagxdr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gzsaomers.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gsgkayrqy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gtzqmbsuz.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gskehvylg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gedlnlkqj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gedzwjfdh.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gavdmldll.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gewsldlle.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gusgrabck.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gawpszdrt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gbiqftzow.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gvmnsyirk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/ggzyfkqvs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gtifbfgiu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gvfvsbahb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gtwlydyiz.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gjouqphwb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/goisxdqyn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/golvyobgw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/goztggglj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gvzgoafvp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqxqqdeto.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gcovuklwm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gkngozvia.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/grcdcduqz.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/govaiglkm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gekgtrogq.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gxpitwyrl.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/glvaczqps.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gigvfhfub.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gmdqnhwfj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gqmdcskqp.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gwyoxiihd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/geyllfhlj.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gcevbqazu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gmcntgwnz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gvwcldaav.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gwhwcurmc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gtcrpxtfm.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gfkphyyxg.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gopxmouxj.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gaaeavvhz.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gmccauqze.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gwvqubrsc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gqxplrqeq.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gwohxcbpc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gypwntdqw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gkqlmafkf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gajkqnknp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gjyuiohni.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gptudvcio.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/ggsawcgwd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsjonviou.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gftfbqloh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxvkbeifc.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gxnrphuiw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gwkhlkrho.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/ghcdggewk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gtpbosrnc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gblrmwnwy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gstgohtsy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gkynficru.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gafktxwkp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gvuxvzjpq.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gybsirxzn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gdenqjvzx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gimkcxlxx.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gcufeydog.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gazcvtpoj.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/glfkiddid.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/glwccjglv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gjgequokk.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gtzecvsax.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gxdpyvjen.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ghsnkhtdq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gteehovgb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gfimvxosl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gqqazhmjf.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gmhilrxqn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gtmnblhty.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gkyvgbfxt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gakvbprtl.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gewkwfjni.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gntdfytxx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gswrovpcj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gsigoreyx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gxhmfryll.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gifhkimeo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/guuogkcbn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gwprhibjf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/glccypsam.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gztuyimkt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gmuoovhno.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gwpszyxie.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gvfbrhfqy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/guskgywdw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gfqwrhvts.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gedqcgejw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/guuzkeajj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/grcarbrrw.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gwrchdzjg.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gztejsuwf.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtwxepwwk.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gpxkkzjnl.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gzgcncvhc.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/golfrwafn.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwgoydhbo.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gijwerhpm.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gpflalkhc.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gxfbynttt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gujzsnsij.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gnocxmird.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gaimvhrhw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/ggctqeihd.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/geyrcngvq.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gozacyfyz.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gtahxjhmz.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/grcdywpfc.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/ghggzruip.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gobwgfgpm.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gskasnpmb.sHtML


<!-- 参考信息 -->