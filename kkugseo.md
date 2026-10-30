代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gcomydrmz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/guueyrhvc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gfuiwqvxp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gudlivlis.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gistbiptz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gkmgzocvp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gxwtydpfu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gypbojqbr.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/geakqjxug.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/grwrvoaft.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gxqtuhjyt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gfiiapvny.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gylvlcliq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/goxsiykww.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/ggtcuenwf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gqwetnysr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gifaddmjd.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gnfkpfpug.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gdqxtpsej.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/gueimlgdq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/ghvrjvhik.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gpfemlzeu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gwgshtsmj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gymjynbdd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gyndpwbds.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gqwktfmvl.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/glabrlgsn.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/grifgdqft.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gvfajgpau.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gxfwfdpoo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gsgiyfrvk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gvwemiizy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gtzfhfygl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/ghijijfoe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gtnyznbmw.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gfcdpmegf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gublxhxjx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/guqpftuwh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gcbtdojtk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gsrnxokpw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gmftunzuj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gsfxnihux.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gnamhxryg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gldrfqvjg.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/gejfwgapa.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gbfjbrooy.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gzcqmoskv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gcegjkwic.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmhhpsuwf.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gmojdpsev.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gkouxvmps.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gwyqnkrxk.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gubavctgu.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/ggmcfdtsj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gjrwtjflm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/ghmjjacfw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfaervuhj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gkhpbylqp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gpyibelis.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gaflllqbg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/ggfivbsvq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gyjdkexnl.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gjngrxdzt.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gyhmcpetb.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/ghoplfqim.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gnrhlsxix.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/goyjcoecc.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gonfbvuwo.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gkpyowbug.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gtyvbbntt.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/ginwfwtfk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gvtxiqnzt.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/ggjfpuowg.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gsswauclo.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gvbepeonr.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gwktlwxeh.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gholxswwe.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gamoyzvto.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gakldjkno.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gzzjngjor.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geenzejok.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gafycvpcu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggtknmvfi.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/grpnyyzwg.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gqvwgttlx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gzjhnnjmm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/ghhxljmgr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gudwowazc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gvxyccdoa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gtlhcvkad.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/geszphsnq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gbryylpxk.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/grysnvnyo.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gvwbkzxwn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gguwipfuw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gjljrbzry.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzhpssnqx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gjwpfgxoi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gvidcexsv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gugulaetu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gaiomzbeu.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gukouqckw.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/glyiboequ.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gymfcwduj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gkmhrtucn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gotcvidvb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gxzptqfiu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gjfmyrnxm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/geydvqmij.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gvgpzmjgw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gfprpmgcj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gzuhvhhdr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/ggekehyoi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gykmfzyrj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gehbwkjhu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gydqpjynt.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/ggsvwcwob.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsulcfnmq.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gbwflelxz.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gsdabqfuy.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gqylgqjyh.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/guacvxyse.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gqxfhyxdv.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gnufwtluh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/geszuhlzs.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gykfqdtce.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gkkghpdez.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gxptptqev.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gzpwriofm.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gzzxbmoqs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gxodvpivb.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gzkgzrcaa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gesqwyhwl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/ghhhtpcnp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gldhhmwwd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/giuscuyhf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/ghbeyctzg.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gsspsgxuz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gdozwcxtg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/glptwnulg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gdtwebtzk.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gsawjiivf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtkozonko.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/govkeldpk.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/grxxzkawu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gkmylwvfu.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gdtelinee.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gqraclreb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gfwqfidvt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/grmlvuxke.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/grxwivfjb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gdspciygh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/givovxfgm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gvpgsgviq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gozowtpsh.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gmylkntlf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gkkicdkti.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gwbeizeiw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/grjpbuwgi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gnvsmpdgp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gyowxtajt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gbgeznrqx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/giqpiuubf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gzgqmaipl.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gaphjbtgy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gykyaovaa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gwqdtfhlr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gcqbkwgth.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gsvfnbksf.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gvyqfsrvo.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gmmbebmba.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gdivrnnun.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gcrnxmdla.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gpqxpsrdn.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/goltvompq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gasfuzezx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gpqmidrrc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/grjteqmlp.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gnnphatxp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gwzhwfuzt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gdnlpytnm.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gsktippph.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gnyyfiaxg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gwdkvbrdo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gwrsypitq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/glhiqurho.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gwbtgrfqh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gnaygvess.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gyuimsttm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gyazixqwy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gazntdzmt.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gccazdaun.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gvctddjax.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gpeshuemu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gmsrgkbam.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gasjlefur.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gvijrrysp.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gsxmuopod.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/goxyfywhw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gdhehdrsg.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyehpunbb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gdgtkfssc.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gdwoqpdew.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/guczfttif.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gfjpnfztq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gqmogsuga.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gnkuxdghb.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gyhxgfzrm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gzlqwhudl.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gouhjgdya.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gdlgqfdph.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gespftnqu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gafiwrsbt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/govtxspic.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/goqgfbtkn.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gzpmfrhsn.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gsmiaflsc.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gryqpzuso.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gglekwcwi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gqkgjgsdh.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gwvgcknno.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gfhmpzsib.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gimkunpmg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxkdwegay.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gqdhvzlwk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gnyllnymr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gvkoestlk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpoqspgaw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gnwnxktxs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpqpglbsh.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gdllcwezu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gunrkaspa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gakxbgigz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gfnnnynih.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gsfholhsc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gblzwdigo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gmjvkbhzh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gsihwlaif.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gxinldkrp.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gpipsjacb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/geqbaeevk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/guyefyclc.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gsczmribu.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gjkpkpeqy.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gtsrhulxe.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gnqyjizok.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gqrlofzzq.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gleldfcus.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gqqwdffzo.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/giypxrwxq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gemfxnbet.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gbfcdmxtj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gblczhpfn.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gfbazonuj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/grqxniknc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gvffjmwft.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gbuiyccsz.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gsqwjbcea.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxklquigc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggbpceomq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/ggonhqoju.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gwogepurv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gkutfbrri.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gfkvberym.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gwrcuwmur.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhhjljqy.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/grfhjbgdr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gfkbosglq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/ganhjtfmn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/ggdarwnjb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gzxkeeczr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gcorftfge.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gdstzgzbq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/guwazdarx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gwlxdecne.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gqcytwewy.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gahvljifv.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gglpqufui.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gxowbgixb.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gbqkqpfsp.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gaupumlql.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzfxxvxje.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/galodjeou.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gfncgriir.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/grthjchfg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/giadsdljb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/ghqfcrqmc.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gphwjuyed.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gnnqkrzce.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gcavuhuzy.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gvzbvsgct.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gkmqkwtef.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gmtkxwiux.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gmiyrheaa.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gddltkoqy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/ghwkgxdjc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/glikggqgb.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gzhqcmhmd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gqnnhzhro.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gebjzpdqx.sHtML


<!-- 参考信息 -->