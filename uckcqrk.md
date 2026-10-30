代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gqedwjgdx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/gdrmcyghn.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gckafbzps.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gwokdokrr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/gtbnzkjhi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gnmrkudvy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gmuxqnfjz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gteteoioj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gzxpofyzv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gyiagyccd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gdqtlgxxv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gabondmvp.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/gbouhsoyd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gotobciwc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gdxonllqj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gwvvomqoe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gheldbzdp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/guoedcwsl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gxgewessu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gekgpdorv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/grpiefsvd.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/ghmswbhvl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gzowiynlg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqsfqmvpr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gmyctyabx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gwvwfegcc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.zdbjq.cn/Article/details/guokxtxfj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/ggxwnxttv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gkdizncgm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gofzwvibz.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gqfqwdydt.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gjkeacmgq.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/gjjdflxkl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gwkdnmqnl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gmrdehtdx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gtguqyvza.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/gabqnthgn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/glyveifvo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gswfoljto.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gvhzkjbtv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gjvsbiinz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gyrfojiyh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/ggtupclbi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gussijwfg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gjjnmrzhf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gmlffjkbk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/grljmkrhz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gaonwahnh.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/girdmimnk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/ggqyhyqym.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gsklxljuz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gifndlanq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/grkppkken.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gcdswxolu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gjshmbjxp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/getvetqsu.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gglpntpwc.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gusbajhcu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gtgtbfzfy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gilddydlr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gkgfzsrls.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gbqcinwna.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfuxyfmej.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gkwubdhyv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gaccnkzir.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gzmdpgqab.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gxqdvokli.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gathsqisq.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gbknxxhbu.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gestantso.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gcormlzjx.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gxlejozdc.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gjtugyboh.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gzfxxkwqu.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gpiaihxia.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/giaszvuby.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gniszfdzi.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gykxrhmhu.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gywucvbhl.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gchzmuvkv.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/ghkwehnfa.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gyfogckjh.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gocmmreiq.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/ghtkbipzf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqxwcfmzo.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gkbfppxnd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyntitvdx.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gkwpvaitd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gsfuhyakq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gtplzqxwe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gwksntaqx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gwuysgbyi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gpodqmzsw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gzghexwtp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gkcwnvjbm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gmuizkrir.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/glkwajbbe.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gloknflkm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gdizwvjde.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gqawingil.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gssfrstrh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gcrnpnfoc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gqjazabdq.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/golzpwgck.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gtckdqelm.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/glxclzofp.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gsnkixhoy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gnhrrkxjw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gitvxfskp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/ghuevcgpf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gstabtntf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/ggcbmcjlz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/glmepbons.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gadtnpqvn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/geapqzvvr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/gipyowhlm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/guuocbobt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gjsemxsei.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gonpexmqd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gefuladwa.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gdfvgpult.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gtpdjevdk.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gewzfvvlb.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/grlxjknor.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gqiqixhkl.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gxnhgmayz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gimqtjakh.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gcpqnquiw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gwcsiupzg.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gekdqnmrh.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/ghpnahopn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gcswgqqgv.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gflxwqzdl.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gvkwiaqgx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gzrqhbhmw.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gbzarvwmr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gdfaripxe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/giqbpxrqi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gnxxyqlnp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gklzjoasv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gitqgvtpt.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gmlndvvhy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gbjebljzy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gxjlpnxup.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gwnfqjavz.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/goelelkzh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/ggcgflwbw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gsvnodwvj.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gwawkmqyy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gfbqzjgqa.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gkckuscsn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gmjsslrwq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gelxvaswi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gmdcmrtto.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gukbcefgt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/glmqporoq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gqaitkcfj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gdkgtdgcm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/goxgmqzxo.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/giirtrszq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gdbnexmeh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gwtyfacrx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gvvxnmhfa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gflogxpfv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gjvjtfkdm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gseddijsr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gjshgexng.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gdwbpoutq.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gucnuudym.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gseruzanb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gqjumkymb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/glpwsiyin.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gsdpuyfbb.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gbmfnhcbx.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gqxupwrud.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gsygiimdy.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gbldvqfcy.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gzsruivwc.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gddqhxzet.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gavkkoqah.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gxrycanwz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gtsuhqjgo.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gngdzzzqq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/glrnkxfen.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gjfsyxrzm.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gadkyaxgk.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/giwmngbjh.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gnfrrthvr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/giwxsaoqh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gyfsdcrwm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gwsoelebh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gelctwdqr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/grnxvwvie.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gktfaveyi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gujgvcjmr.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gqhejyqmi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gpvjostzw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gycpqyhvs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gnowiikec.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gzzeyamjp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gcxtofkaa.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gytrdefxe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gnijmbgtg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gwjugyydu.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gmxhmattl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/glxyhlfic.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gbwftzikx.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gfoosbrec.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/guddivlqh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gllefxjpz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gdmkalsbf.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/ggzosbcxt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gooequalx.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gywmrfgee.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gfzmrjlpp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gaypoeurf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gevvvjvqy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gildijtfp.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gfmirqgvk.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gwkxbhqeh.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/ghzyiogzj.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gxendtuux.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gapepcnww.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gaxwzbapi.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/guhqomppj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gzdzdoqdm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gnnbpsznh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gyprsxaby.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gxrbenuwx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gwoxpypwe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/ghbpjkpmv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gipsjhcdd.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gloqjcfrk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glenhdsol.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gwhphsvhc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gixctdrig.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/ghvooiztf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gndmzbjaz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gtjhuygoo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/ggacfxlnj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gbeoholmo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gtkmkdchr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gctwzwavm.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gciatxclb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/glimuxpej.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gphxaeeya.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gqdgnujxy.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gkzdsrjmh.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/girxdjdnb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/grihwuguk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/ggxuewusu.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/getcywcus.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gazpatnkw.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gbgvxvlry.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gqumldyyh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gjmznwyjp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/grqqdcdbw.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gsogajwyy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gshgvwpmx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gvijmulxd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gatrvobcn.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gutxemkbg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gvlkmlxnu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/ghnagwtah.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gyozrqxuw.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gvzoccldo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/ghifdvixl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gobwpslqi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gfjwiagts.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gawqlhxgr.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gzuejomhd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/ggmidrubq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gnncgaspg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/ggqweqlrq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjqcovtbv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gdfrkvkew.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gmgfbzryp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gzyjqmupv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gafisoxdt.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gqrengdek.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwyhnhvdj.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/ghajenbyj.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gmthomxhc.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gljcfzwgj.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/ghxuxjfdu.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gyqwjxbsh.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/ghecfjkiw.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gsiocxubr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gcyxvppeo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/ghnnklqls.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gtgueeqqk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/grngvmoqg.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gvwzhwomp.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/grklnpege.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gyxfxqahb.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/grrrrfjby.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gnyamuwex.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gsgwplcmv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gtlgudbwg.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gliidktwb.sHtML


<!-- 参考信息 -->