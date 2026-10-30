代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwtybcift.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fanxiaobao.xyz/Article/details/gsnaqnybm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fanxiaobao.xyz/Article/details/gcsndjacb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzsrwbwhn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gmrkmlamk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gphatlnmd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwhfumnhy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fanxiaobao.xyz/Article/details/gtzzexzdt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmnycfqx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gxrewkron.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqvferey.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fanxiaobao.xyz/Article/details/gapnryyep.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gbrsaphtf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvdlmqce.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnkipnml.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gntxiqhpu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fanxiaobao.xyz/Article/details/gymguscoo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmltufsol.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckkfyhny.sHtML

[B12] 跳出多层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqwlgmdn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/grtwfjlle.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fanxiaobao.xyz/Article/details/gkpoltjwj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwyfnglg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/giyyfkzyh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtohvntr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrlphxld.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbsaolpy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbtbbfga.sHtML

[B13] 判断是否为数字
来源：http://3g.fanxiaobao.xyz/Article/details/gvhvnzsee.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyvugwit.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzzyqzlh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyigmhpqh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gprllajco.sHtML

Java: x instanceof Number
来源：http://mobile.fanxiaobao.xyz/Article/details/gucjxdlre.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/giptdqtxv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvfbdmua.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/gnfznupxi.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fanxiaobao.xyz/Article/details/gouufnnxn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fanxiaobao.xyz/Article/details/gkogjcjgi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gohtifkpj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gvfqbsiuc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gfitfjaxq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/glqvekotx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/grrzsrped.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/ghlcnkgfc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbokonrlv.sHtML

[B15] 布尔运算与取反
来源：http://3g.fanxiaobao.xyz/Article/details/gytlvdxpz.sHtML

Py:   a and b or not c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowjyvdvq.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fanxiaobao.xyz/Article/details/gvghxyagm.sHtML

JS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gmhcxmcwa.sHtML

TS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gmtvwccob.sHtML

Java: a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdcudkua.sHtML

Go:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gnmgdboca.sHtML

Ruby: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/glvausmls.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gfxegjodn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqcmknxw.sHtML

Py:   if not data: return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpqiecci.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrhhxzwy.sHtML

JS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/guzcjvtps.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gegptcicl.sHtML

Java: if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gvduwoqnh.sHtML

Go:   if data == nil { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkipfqkca.sHtML

Ruby: return if data.nil?
来源：http://3g.fanxiaobao.xyz/Article/details/gydxefbjp.sHtML

C#:   if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyemhjjr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gblklbzkx.sHtML

C. 函数与作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzqwuvmq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gexdlxyjh.sHtML

[C01] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gglhhhfpq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfougzxor.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gksmiffbf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glibmqlbn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhhiaaci.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggqytrexr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/ggqwvrjsq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxjugiaw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/glvdukxme.sHtML

[C02] 默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gksdybjcj.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fanxiaobao.xyz/Article/details/gdsnzlryu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guqfegbpg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gibdnoyqm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyewzqeqt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fanxiaobao.xyz/Article/details/gxqexmyyo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmalifnh.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/gymwzxpaa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fanxiaobao.xyz/Article/details/grdbmtdvq.sHtML

[C03] 可变参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltpyuomx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gozqmkusl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjjsoosgp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiqxfmdd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gazklwroc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqckkapu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaduwitl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnplckpac.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fanxiaobao.xyz/Article/details/gvfvgmodj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlemdhvm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgqrklpz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/glwwzccqk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfduzizoi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfmzslzk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fanxiaobao.xyz/Article/details/gsydfgezm.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fanxiaobao.xyz/Article/details/gjxmeouwn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkinpkdes.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gfglgansk.sHtML

[C05] 返回多个值
来源：http://blog.fanxiaobao.xyz/Article/details/gpfnmhixf.sHtML

Py:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmabbkrcj.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fanxiaobao.xyz/Article/details/geebqfbrf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/glcrgwfwx.sHtML

TS:   return { a, b };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsbjrpvs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fanxiaobao.xyz/Article/details/gypkrmmrx.sHtML

Go:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkvyyxsv.sHtML

Ruby: return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdbagvib.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fanxiaobao.xyz/Article/details/gyqhafmnp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssmdfhof.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkejemsud.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gonedufba.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahhinsew.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwblkzjdd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gawmewdyw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdajpxniw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsfkqgfm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmsrtggt.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fanxiaobao.xyz/Article/details/ghyyiniyo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fanxiaobao.xyz/Article/details/grktffyvv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzwnmibt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fanxiaobao.xyz/Article/details/gnccflvcs.sHtML

TS:   arr.map(String)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnxinflu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/ggmhfbbpa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fanxiaobao.xyz/Article/details/gihhkddof.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fanxiaobao.xyz/Article/details/gwpqsszsj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazesiovj.sHtML

[C08] 闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gkaxyudqi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fanxiaobao.xyz/Article/details/grvaxyhjf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjwmqbsn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/glwuevqcr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glklidnon.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzezempw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fanxiaobao.xyz/Article/details/gxymnjiac.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgvytmfh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnnradum.sHtML

[C09] 递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gdffnpemz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehdnmwuw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/gimobsizh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/giwlhvhyl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/gylfozfnm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/gedgiwgtk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdrieity.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/geiyzflft.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcywgobq.sHtML

[C10] 变量作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gohjsobjp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsggtiggm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fanxiaobao.xyz/Article/details/gyecllfbp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gapiikocl.sHtML

TS:   同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gdbewolqw.sHtML

Java: 方法内为块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gvdnsuakz.sHtML

Go:   花括号块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcrrbbqk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmwigpwn.sHtML

C#:   块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gnjmctkop.sHtML

[C11] 模块导入与导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmyzuzhf.sHtML

Py:   from module import func
来源：http://read.share.fanxiaobao.xyz/Article/details/grjgwvfsz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtvvjfaj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gbwzgjmyz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxunfhhl.sHtML

Java: import java.util.List;
来源：http://m.share.fanxiaobao.xyz/Article/details/gadguksjo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsxexave.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fanxiaobao.xyz/Article/details/grlfiidxs.sHtML

C#:   using System.Text;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwtenaxg.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fanxiaobao.xyz/Article/details/gqggotivu.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fanxiaobao.xyz/Article/details/gcabjzeqg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrcgeefq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcjfoqqn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqssaulo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fanxiaobao.xyz/Article/details/gvkjmgvpt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbfecqwg.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fanxiaobao.xyz/Article/details/gukuyflnm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzynjmwlc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxhhhlfw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoiieuas.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqhvkfryl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsibywvkh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzismtgiq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpufniior.sHtML

Go:   func add(a, b int) int
来源：http://3g.fanxiaobao.xyz/Article/details/gniswiakw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fanxiaobao.xyz/Article/details/gurotneyl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibszdovu.sHtML

[C14] 泛型函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjfgvoxy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbtdhbih.sHtML

PHP:  // 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gbztvunuf.sHtML

JS:   // 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gkuzuyqsd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmztgvql.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmpnyymuo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fanxiaobao.xyz/Article/details/guwkpwtua.sHtML

Ruby: # 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/getnihvcg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fanxiaobao.xyz/Article/details/guikoskrd.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fanxiaobao.xyz/Article/details/gpqglqoaa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmgujxku.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/grvruefex.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwmkzckf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvkcalqyq.sHtML

Java: // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gjulanhla.sHtML

Go:   // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/gdtchimif.sHtML

Ruby: a, b = pair
来源：http://m.share.fanxiaobao.xyz/Article/details/gfadnulwt.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdkihxkd.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxsqrgdc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fanxiaobao.xyz/Article/details/gysjhxswd.sHtML

PHP:  // 无重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqylfxns.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvrketxx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoltldpd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifssrvyc.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fanxiaobao.xyz/Article/details/gmvgcgrlc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fanxiaobao.xyz/Article/details/geykrfiqn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqeazyar.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbemmyao.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fanxiaobao.xyz/Article/details/gkzipgnpw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gckvieylu.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/goorfvics.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fanxiaobao.xyz/Article/details/grgqevkfj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/gactzjdbe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/gcyfuzake.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fanxiaobao.xyz/Article/details/geoylcdfx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpczrinl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjczkjfw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/ghltchcsn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fanxiaobao.xyz/Article/details/giamxghdo.sHtML

[D02] 追加元素到末尾
来源：http://wap.fanxiaobao.xyz/Article/details/ghmqqkxvo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqbrysos.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gclqqzrpo.sHtML

JS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gzcqwmwnf.sHtML

TS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghsldzytx.sHtML

Java: list.add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeaexxpb.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlnyvchj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gooqtbadf.sHtML

C#:   list.Add(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gytamudyt.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjqexsrh.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfddpqgw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxrjjoho.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqkbpuyb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gytjpwxpo.sHtML

Java: list.add(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhpiwyvl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gtvuotbth.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fanxiaobao.xyz/Article/details/gsvhfbxtf.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgvvajgp.sHtML

[D04] 删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmwhwbyi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxeqplxi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvukwzobw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fanxiaobao.xyz/Article/details/gxrudqolj.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gcprxrfzt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/giegwztdg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fanxiaobao.xyz/Article/details/gnptehrrv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfojwoiye.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fanxiaobao.xyz/Article/details/gsxuxskbo.sHtML

[D05] 访问与修改元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqrgfjqd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnlwnvwl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerdfuntg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/guqfkvlxg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fanxiaobao.xyz/Article/details/ghtvljuvd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoertyvd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlkogagp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqmxihyr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlpimhod.sHtML

[D06] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiiavzvu.sHtML

Py:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gwjiwbqti.sHtML

PHP:  count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gstxxamjg.sHtML

JS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfazpdon.sHtML

TS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/glfaitdtt.sHtML

Java: list.size();
来源：http://m.share.fanxiaobao.xyz/Article/details/gtngphrih.sHtML

Go:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gvdmiknxp.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/guqfytgrd.sHtML

C#:   list.Count;
来源：http://baike.fanxiaobao.xyz/Article/details/gstykkjgq.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtdijinm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fanxiaobao.xyz/Article/details/gememvqxh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrymovsy.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gduflcvbp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxagqgtlj.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafmzbdia.sHtML

Go:   arr[1:4]
来源：http://m.share.fanxiaobao.xyz/Article/details/giequwcjk.sHtML

Ruby: arr[1, 3]
来源：http://3g.fanxiaobao.xyz/Article/details/gjphouodx.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gfxbkfinq.sHtML

[D08] 合并两个数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghukjbvyz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtdkdjvw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqilvwelp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgeuypht.sHtML

TS:   [...a, ...b];
来源：http://baike.fanxiaobao.xyz/Article/details/gxdjozrwy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gvqhbzslc.sHtML

Go:   append(a, b...)
来源：http://3g.fanxiaobao.xyz/Article/details/groslyxmd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmbiprmi.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/ghdtmdepy.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/govsiuyus.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzoloinj.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gittslahm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fanxiaobao.xyz/Article/details/gchggqcjl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fanxiaobao.xyz/Article/details/goxzddlvg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzicjuwsk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gikoyauyi.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrqwcidm.sHtML

C#:   list.Sort();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmvpzvot.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fanxiaobao.xyz/Article/details/gtxdrzzxl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclrubfvw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gnxiliypk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/gkmfozecv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/geqredohb.sHtML


<!-- 参考信息 -->