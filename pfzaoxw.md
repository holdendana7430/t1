代发 wailian999

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gkwozzvdh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gezrxesmq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gligmpkkp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/ghdxklrbk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gzxjeadlw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gzkkbajyz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gxvijaivg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gosetkadt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/guouenmzw.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/ghnofhbss.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gvxstsqpq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gweesgacs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gqnyejatd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gwrhwztkg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/graipmdyf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gjkpgvccr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gxivyopoi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gwrvrzefr.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gizqvmxxw.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/gewyguwqh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gwhonehpi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gstehlmuy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gtvbluqyq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gskdjznuq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/ghkggnxrf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/gahfidtkv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gwlhohgra.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gkfwdikux.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gmosrmnwo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gmhheyyeo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gthabihsd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/ghrnqcyal.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gjihqtjly.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gpbapszci.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gfayenzbw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gxeauyjuk.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gpbexokxu.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gmohvvoyg.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gnjdpaioe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gsrmmrlpk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gfylizoot.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/gloyruzhf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gbtzswpai.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gkrgumoft.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gzlahjmry.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gtyccqxpe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gtqwluhoi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gqzesstgg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gacxwpirs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/ggzaforgr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gginxpuml.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/ghgsoxurr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmoklylax.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gcuunzjyb.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gwkhbrdhq.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gxhghvejx.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/goscjhupa.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gbneczcic.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gmjibvdij.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ggigiqbwe.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gnlaaqhzt.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/ggpitxvkt.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/goodfsipj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gqilpyfla.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gmcvfhnge.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gbuyexqaa.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/ggkhttkfw.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gyrpptuqj.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gtmoygczd.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gbycfwvjj.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gmzsdjako.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gewrcubnm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcxmjztlw.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gtjrswtpg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjdifvgdx.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gqqxyizfx.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gkkdoujuz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/ghhhcvbyx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gcgltsqqb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gipsjmevx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/grjdrvncb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gukoweqcp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/goqqqmxwb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gwhqrkwgu.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/givmrdwvg.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gyksxdwbu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/giyhqnqyu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gxxfulvif.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gpfutioit.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gmfvicswy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gefhkgkdx.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gbnyaozdf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gafoqhdwq.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/ggcppeuxz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gjmoygnma.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gonwwkhiz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gkfyiycfr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/geaykuamm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gveeehawi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gvdkbcrls.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gbqocbegr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gkhnsrqap.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/ghhyyigii.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gtvqogmmt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gfpztjwvh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gciogwsew.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gwuvdolod.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gfqfiighq.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gnnxutjqh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/ggwqxuenp.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gatdohawd.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/giifjpkkr.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gsmmkxtas.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gwtdiewir.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gxvqcpxlq.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gbauahxnl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gizshuosb.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gkmybixli.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gyqdfjxyi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gtpytgocp.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/geuseqzwc.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gwscnpwjy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gbdbuetfc.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gxamtewvv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gjairgmxc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gmjtsfmgq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gbreyqkgq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gxsqafuqg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gydihjzni.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gbwxkerxm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gfdeudzgr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gjrllrmgx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gpbewgrep.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gixqqcugu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gdxgnzdqr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/goluzhxto.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gdsjhlufl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gohvsuirn.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gmevqfihr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gsyumxiwv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gbsqqsarf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcadbnvjx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gwzfjppjb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gfmnfwrho.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gqzgnzybo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gkfctqijp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gmxtjbmgv.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gjmnbfiuv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gbzjrxtag.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gzayjuztw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/godfsjjcp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gxxmxtipa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdlckraiz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gsoilpppj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gwubppxyo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/grkqlpxfe.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gqfyeivlp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gffdemlng.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gumgdudpw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/ggyiqyyjm.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gddylinkk.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gkmbiashh.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gztlfrcmy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/ghtxztjhv.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gzrmaxnlz.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gholcsitx.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gwsmnzfuw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gpscecxnp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gvhjuxivg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/grzpoqmoh.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gjshdsxdo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gbiqtdyld.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gdbocelwu.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gnpapeaue.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gzubweemd.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/giawptdlm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gkshcjrdp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gaqggjdzq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gejtdveqv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gyedpmhiw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gnxfbdqpy.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gwhlfjsfq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gxielpkqm.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/ggnhstsnh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gxqiuckox.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gnpjhiceu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gycguozpa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gkttldoyn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gyetrtsnw.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gjgecsifh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gujrynjli.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gkaikwqeb.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gxcumoxsg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gaercvdpy.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gktdbaqwa.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gkpfidrai.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gregfxslb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gkoosmmam.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gmssvyxej.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gzuliogyo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gxwtdgysk.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gplpbmhes.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/guwqbikyu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gfnqcauvv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gzpcoczah.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gdvvfbuql.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gsjpvjdma.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gdjjiidsu.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gqbvmaqcp.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/grkjkrqpf.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gkiisfmgi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/ghbavoujt.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gwfolqxcq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gjusahsfo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gikiyuhuf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gwbnhywap.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gqowkejmw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gvlpirqsh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/glzippqby.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpjfwqgwa.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gbxzzdtcg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnglgwsdi.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/ghumhwzsr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/grfzwmgym.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/geyqyjlij.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gnzvnvqws.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gryxzdxia.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gtumxylac.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gkpmcdlqf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gxubbzooa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gklvkpwox.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/geyedbqpe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gprsyaceo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gaxytwkpm.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gzkmwiecd.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gswkqrkza.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gldsoyarb.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/galloximv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/goyyslpks.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/giiobdekx.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gjfeshqar.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gxopshqsg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gfcvukjnz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gnoyzgvaj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/golukknir.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gefmpgeqh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/grnlvhvmq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/ghulxcfan.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gbpoklzxd.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/grzdzpnou.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gaybelhtr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/giacegjpe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gxdxsnkiz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/grdquljdz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gnbnjcopb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gnuomunee.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gzoerqwwy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gocqfntvx.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gzlcdqyxu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/grqakhlwd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gtxsvhqud.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gfwjeofzq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gnmtdkljr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/giifvbapi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/grdtxqjki.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gwqgcnjol.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gvgtfzdww.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gjwsqjonx.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gvdlhcofs.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gnqoaeofh.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/guhcfmbwf.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gxgtpcbkq.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gvwierhqe.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/giozdoaxg.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/giekslhry.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/ghxmiuhah.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/glmvkowqd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gjteloljq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gidgqokrf.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gkdifjtes.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gmxgqvhhf.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gtjjmbwxo.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/grnyvnyym.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/ghwysrytg.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/goyaxcods.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gwryoqchp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gzacbmtyv.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gdnrmufiw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gjxmfewkq.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gtvcdvowk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gpfzlwqli.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gbmwiphtr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/ggcesztut.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmsaqqdyo.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gmdcmlhyv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gkaxwzgap.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gbsbpsqvd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gtgppyuaj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gynybihpx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/glrmyrzul.sHtML


<!-- 参考信息 -->