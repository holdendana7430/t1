代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/gqjuehavk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gygnzfdqk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/giucinwqs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gapqifomr.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gysfrszso.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gqbnhgywe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/ghsxqfxly.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gvglsxiij.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/grlnjdxel.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gkpdtmpls.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gmnsvtjmf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gniqysvtq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gaoucpfma.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gmsjwrofr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/groolkicd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/ggaxzdtyc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gcdjosljd.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gbfzvziao.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/gqcyokkwn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gvmqpahzg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gtbcdwsjy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gfltbeqst.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gifyaynxb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gxzzldiag.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gveznrtfi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gdctqlhvk.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/ghtjqfklh.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/glxnjszxm.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/grqgsmtra.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gphqzxiin.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/ghxuogqyb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/ghqvesqmh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/ggptupnth.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gmffiqmfi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gshoxbljc.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gzbhhmmhp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gbjgkjacf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gjjuhjkjh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/ggkjyipzy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gxvlshnor.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gsdzdxrgc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghshwzxry.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gvytqhrft.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gevenhjlu.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gtmccyilj.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/ghzkwhubj.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gfhdjgdtm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gjbbdchua.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gqbfisopn.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/gvbxceccf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/glekkzrsb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gczfpetmc.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gcrjphzfu.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/guccfeqkh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/grypxnexm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gesxutsbx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gjkwtuhgj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gmndeyakl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gmklwqejh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gakzlhtme.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gutgcivuj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkvyaybt.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gkmqhnndz.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/ggmzlyudt.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gbfassdfk.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/ggnfifhbc.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gnmunqpro.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ggtmvvdwn.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gnggidqqs.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gqxbribry.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/ggmkxtprs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gngalpctk.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gqrbgaizk.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/ggonstckx.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/glfbvzbuc.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gsgenocfz.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gpygrdhdn.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gcyaywcmo.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/geowfrukm.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gyqqvimna.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjtyhbyjt.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gfluqvbpc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvohfblvu.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/glltwyqrz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gbvviprdl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/guveltfkf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gntmzcbtj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gkazxeymk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghfiidkma.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gcsxdtwlb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gkivrwspb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ggflfqwna.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gkttgpeny.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gotjaohom.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gyghwgyuo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/ghkswygkj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/garxgajnb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gwtaddiev.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gvbrojexe.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gkinwrarz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gfrocyqut.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gkgvndprn.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gofzosygo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gmuzsbjjs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gapuqtmri.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gmhlcywqj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gferijxac.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gqsgmngpk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gaslpotnb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gpebjbjez.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/ggtmgwhdn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gdivvltbu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gbkmwsmhj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gqhiaoisx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gnmzpmwzl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gruirzmsb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gyxigbnwz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gdtsafkpk.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/geondijli.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gckrfhuug.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/goyzplher.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gndbsilng.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/guaxwacob.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gfghibzho.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gjwmwwyta.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gfsoihmml.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gloijmrap.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gbwislysz.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gilkkqnsq.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gqqenyiys.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/goswtgwch.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gtkgtgznu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gqibzpxyu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gnavracpw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gxwqslwyx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gxmmmciqv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gtczgfpxr.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gwzzmxidi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gcqkxkjow.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gypygoybm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gevaquftb.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/ggvhzzqkr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gxnudvomv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gwbgqimbl.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gnxyjttbi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gkffeebyz.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gyfmzyxnv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gyzhuvmyi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/groxyoler.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gkmsecyqe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gfgfislpn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gznfkgcty.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gsmqpaduj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gfunuimad.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gywuneoqh.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/glvmslrrs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gmbkihsml.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gqgzwzxmk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gmbbdyrcy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gegmtbpsi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/goggrnpjc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gtwihbltw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gpwyyaezs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gjlybjaaz.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gezeotaqh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/glphrbmtr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gxnnszvhn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gvhqzzdqz.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/guynsmrsp.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gwebhzucs.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gipycahfg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gfcisudbt.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gdssenkej.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gpbjftdaq.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gwpjawuao.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gtuxlpete.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gspajhnue.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gvqsfcwwu.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gzyifugsj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gmbmypzja.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gjaydxddn.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gnmnvlfaw.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/govzkhspj.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gunppmoel.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gkznqnbbu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gcikuomko.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gqhzwbrmi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gvbonpikl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gfcngqpwo.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gqejycuvz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gczoimgtp.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gzbuzjesa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gylbsaorz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gxykulqrq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gtlwdjagu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/grrnadlmb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gjcqfeefg.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gsovuqjoj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gtopeogsa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gkettkbcw.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gkpfcastq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gfrvlieqd.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/guyskhmiq.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gskucdtij.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gfuigbgcy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gbuogurob.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gjlaicnyt.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/grrvsoaeq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gvogjrdrc.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/galgoydgc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gkzghlbpl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gzremdivw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkgbrjfku.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/glovluadx.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/giooptjtc.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gpamqksbp.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gkemeqgpi.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gnxcfqxqe.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gtfdyobyi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gxxmifsxd.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gamimbdrc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gsexnnetq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/guovvctvk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtqzyekkn.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gakpokzpq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gatqntkoh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gtbhhfqzm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkspuogef.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gggjsdsua.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geqgsvtdl.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/ggfwvtxww.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gyhjlztnj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gyeqjleob.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gcvvdgiyk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gynftvusq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/ggickrxko.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gcbifcono.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/getzhjysz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gvazetplf.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gxgxbtnkk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gdtezudwt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/golltkidd.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gamolvlpe.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gurflqjgo.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gyztqlxkk.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gcmtfzdvk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gibqcylqq.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gijdscmgi.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gfvnobkeo.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gqmomxzle.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gfgmtghrq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gjymmnhib.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gqiwmogcu.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/grzbktphh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gnjfqlrnk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gfcbwlocd.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gsqecqhce.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gnsblwdep.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gpkuauyld.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxiiofghi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gzdxyqswp.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gtheamrmh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gyibjqoxo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gilmktald.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/guplzrxvo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gjyxqcouy.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gpcretgjl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gdxzhydvl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gmvlazrgx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gzbepeuys.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gfhwxbxbv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gqxspjlss.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gurupnqts.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gohswcwon.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gmrxltdqy.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gdkebamjc.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gekcaphip.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gvvrbevpt.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gouhdbqpy.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gzjvyqlhq.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gawmgbchk.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gutqchovj.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gjxbphlte.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gcnlrenha.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gkzyzrbjw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gxuzqizvd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gfljvtphl.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gkackfixn.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gdzehsxpt.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gngauqxsz.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gweeotnwy.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gnvuqbmrj.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gdpyhxxql.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/ginsvjcxu.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gkrejemnn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gcrrqayoo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gboaacwtl.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gmeqlduxx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gixhrftvp.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gmkikgzhu.sHtML


<!-- 参考信息 -->