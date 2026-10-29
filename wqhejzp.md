代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gmsyorayf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gxthanych.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/glywhkwil.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/glwucmqrp.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/glruqenuc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gutmhypra.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gawcqqekv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gpdfpkekq.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gsagbafro.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gsnvjxzcg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gvyahlwky.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gzqkmhcmo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gmvkmloja.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gexunawum.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/gdexettog.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gweldaozd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gtezebjxz.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gvhoksrez.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gvqalpayo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/gihalljio.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gvjowbwxd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gnkbzoliz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/ggaqdbmlx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gvamattdg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gltekffee.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gkvfomqfn.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gvbnsxrxc.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gqwriioum.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gbvdxpxln.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gfxzorjay.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/ggcrehpjq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gmpqtseot.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gbwvpsccz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gnpaaxhja.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gtebrzmqj.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/ghrsaypgh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gvgedhyrz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gnbydagcu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/ghridxutd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/glidmythm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/ghcdjgrxm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gfctmgkce.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/ggnlnriux.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gqplqcufj.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gxvklzfvv.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/ggooxfpro.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gwtwvecwj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gyzazlcgz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gactkjjkl.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gfgxfwkbj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gbxzfkpny.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gprybbgtn.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gnuonjems.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/ggknbgfhj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gsaoyyblo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gjikeacoa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gqlgbmamf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gntgwbnnn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/ggayzxlll.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gnxsoledg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/greupgdgg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/grcnzyzsv.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/geczmifdo.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gsrjgkgjo.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gizffvdcl.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gzqmfsmqe.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gwcckzneu.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gckbagcdo.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gqvotowjt.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/ggnztdkbn.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/guhqvopwi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gdokpolbp.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/galxptbcv.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/gmgxwetys.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/grsaiflse.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/ghqcnjgcb.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gaaoqoctm.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gprsfunqv.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gqjjefspe.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/grfcibimq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gebjsbvkg.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/ghossttqj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvyjmeqov.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gdmeuifsu.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gzicgpjmu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gyvndimta.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/guyasvrhi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gvgajlrcq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gwtphqdan.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gqutpxasj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gzwergzzz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gtslfwtgj.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gprjthivy.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gslsyegfa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/grxmkafsh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/ghkaniyow.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gtqroyfse.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/ggcyvlsac.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gacmqyenh.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/geqfmvzpl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/goltmakax.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gaqvfaejg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gvkdetixa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gyxscxmzw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/ggicxmpwi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gejqwnhqg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gefdxsgss.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gktmoeevv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gmbemjttt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/ghwpojvji.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gknbtsbqe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlrtlisb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gnavkjyze.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gvbbknsmy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gisnpikdq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gxlhwgcyb.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/grcsovkeh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gezmsynhm.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gycjwzzze.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/guibajccs.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gcyzptsic.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gsyfxruot.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gwkhyuyft.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gheijratk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gugxjiufp.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gqwizmeqo.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gyekicbdf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/ghxpsfyjg.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gyysxocug.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gfkeusctk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gquefpbll.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/girstkgyv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gvslmjwmx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gfzuwggit.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gkfyszdif.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gdgawogjq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gyjxclkts.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gsbapuomj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gywmpelrh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gdrzjeifp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/getqqgdsm.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gdismffjc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gwsislfns.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gxnbixcdb.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gywtcravn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gishkwitk.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/ggbwdmpeb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gbbsdeyvm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gkyutaltb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gbbknuxvx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gagqhwskk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gtieczecc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/givadrnjk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gfycvfevt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gyyvqhtpo.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gkcoygzgr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjwfdyrcs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gpfwovtna.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gwtmrcqtk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gsrxrcelg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/geoplskkf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/glmquxces.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gbakpwoxd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gnzqylydb.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/geatglmio.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/ggpyyclbb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gpagknjbb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gyayaqvcg.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gnvsdzihn.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gausuauqb.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gelmsdspw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gqmykapgp.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gdtliygff.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gsebnqtwr.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/grrmvwtuq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gmsvrxtix.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/ggxgqkkfs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gtjrtnlok.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/guwjosdnf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/ggdoyvocs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/ghlkesjpg.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gcekxboxx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/ggiuxszdp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gtufiamlw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gxaztpcyd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gfpuqkaff.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gjzomwotp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gwchpqtuz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/grvfwxobk.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/guggqcouc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gipebjelf.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/glmvhfhgp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gqibzgmqg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gqytqbuht.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gmoqmlcgy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gvqttgmfm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdsriszqn.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gezrsaffy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gdhxvlzpg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gfiqreoip.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gxuzozqcu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gqqkalsze.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gnsxrknqd.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gpjkyzssv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gheocsqbq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gagjlcscc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gdzfxqsrl.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gytdxkvyq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gjxihihag.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gkcsvvjud.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gpvonugpb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gitpfveax.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gtqrriizc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/geblygesp.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gewkbeyus.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gdgfwzjke.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/grzefpraz.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gfyzoskfg.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gfrsgssnx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gihwsjdgb.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gbqaqcfgz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/ginpgjqof.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gqehxvsqi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gbdvyqdwz.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gyxpaylxw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gzzoguknw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gbytiflie.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giubagwzg.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gpldaviih.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gskepzaxh.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gxqgbwawv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/glybzgtrl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gyvbbsduk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gkgetctll.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gpylomkob.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/ggbysjmpg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gasungnkv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gcpmaeell.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/galgawpxk.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gfoydaauf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gmlaabhgg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gkzbexmqn.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/govnmxxtx.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gfbyxjdyd.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gyguqkyjd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/glpkyjedz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/griahdrny.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gfjammufl.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gqsscpead.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gljidqxiu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gokcjpfsd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gwxjbibxl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gcndpmbvc.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/ggwckpgko.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gfdibiwtn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gtknetcqq.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gmngxuvrh.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gveuspufw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gcnpktcla.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gilgcoibe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gwtpelbew.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gkxzkddit.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gjjnhedtg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gqmuertcb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gpnvzvhbg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gbkffvmgd.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gvaljrpmq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gisgfnnot.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/glzgjxzdk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/govsdlzca.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gkxglvpyp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/giqvyhmjg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gkgolxbaw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gwcubrstm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gfpaxdnot.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/guyrwdcdu.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gvpijtlee.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gtomciwdc.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gxikgispb.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gzhztacqu.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gytzbpzlz.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/ggkwlicck.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/grkincfve.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gfjivpnfm.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gemgobfgb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gewoardow.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gezpluuip.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gwjxntjal.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gajymihou.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gyylgsgsn.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gjucuyusy.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gfsspknpx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/grexbnxpa.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gsgklmkbu.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/ggysbseta.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gjvjiuuol.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gabivdumt.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gcsqlipdv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gkcvoykwf.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gxptkmtve.sHtML


<!-- 参考信息 -->